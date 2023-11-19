# L I S P


```
(defun aplanar-lista
  (lst)
  (if (null lst)
      '()
      (if (listp (first lst))
          (append (aplanar-lista (first lst)) (aplanar-lista (rest lst)))
          (cons (first lst) (aplanar-lista (rest lst))))))

```
