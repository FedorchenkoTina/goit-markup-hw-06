# goit-markup-hw-01

/* ================= HEADER ================= */

.page-header {
  border-bottom: 1px solid #e7e9fc;
  box-shadow:
    0px 1px 6px rgba(46, 47, 66, 0.08),
    0px 1px 1px rgba(46, 47, 66, 0.16),
    0px 2px 1px rgba(46, 47, 66, 0.08);
}

.header-container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

/* ---------- LOGO ---------- */

.logo {
  font-family: "Raleway", sans-serif;
  font-weight: 700;
  font-size: 18px;
  line-height: 1.17;
  letter-spacing: 0.03em;
  text-transform: uppercase;
  color: #4d5ae5;
  text-decoration: none;
  padding: 24px 0;
}

.logo-accent {
  color: #2e2f42;
}

/* ---------- MOBILE DEFAULT ---------- */

.nav-list {
  display: none;
}

.contacts {
  display: none;
}

.mobile-contacts {
  display: block;
}

.burger-btn {
  display: block;
  padding: 0;
  border: none;
  background: transparent;
}

.burger-icon {
  display: block;
  fill: #2f2f37;
}

/* ---------- NAV LINKS ---------- */

.nav-link {
  display: block;
  padding: 24px 0;
  font-weight: 500;
  font-size: 16px;
  line-height: 1.5;
  letter-spacing: 0.02em;
  text-decoration: none;
  color: #2e2f42;
  transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1);
}

.nav-link:hover,
.nav-link:focus {
  color: #404bbf;
}

.nav-link.current {
  position: relative;
  color: #404bbf;
}

.nav-link.current::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -1px;
  width: 100%;
  height: 4px;
  background-color: #404bbf;
  border-radius: 2px;
}

/* ---------- CONTACTS ---------- */

.contacts-list {
  display: flex;
  flex-direction: column;
  gap: 12px;
  font-style: normal;
}

.contact-link {
  font-size: 12px;
  line-height: 1.5;
  letter-spacing: 0.02em;
  text-decoration: none;
  color: #434455;
  transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1);
}

.contact-link:hover,
.contact-link:focus {
  color: #404bbf;
}

/* ---------- TABLET ---------- */

@media screen and (min-width: 768px) {
  .nav {
    display: flex;
    align-items: center;
    gap: 40px;
  }

  .nav-list {
    display: flex;
    gap: 40px;
  }

  .contacts {
    display: block;
  }

  .mobile-contacts {
    display: none;
  }

  .burger-btn {
    display: none;
  }
}

/* ---------- DESKTOP ---------- */

@media screen and (min-width: 1158px) {
  .contacts-list {
    flex-direction: row;
    gap: 40px;
  }

  .contact-link {
    font-size: 16px;
  }
}
