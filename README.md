# goit-markup-hw-01



.footer-container {
  display: flex;
  flex-direction: column; /* Элементы друг под другом */
  align-items: center;    /* Центрируем лого, соцсети и форму */
  gap: 72px;              /* Расстояние между блоками по вертикали */
  text-align: center;     /* Центрируем текст внутри блоков */
}

@media screen and (min-width: 768px) {
  .footer-container {
    flex-direction: row;  /* На планшете возвращаем в ряд */
    flex-wrap: wrap;      /* Разрешаем перенос, если не влезет */
    align-items: baseline;
    justify-content: center; /* Центрируем всю группу элементов */
    text-align: left;     /* Возвращаем текст налево для красоты */
  }
}
 
 
  
