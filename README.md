# lista.nombres


lista.nombres = function(bases){
    tab_1 = data.frame(matrix(nrow = ncol(bases), ncol = 2))
    colnames(tab_1) = c("name", "class")
    for (i in 1:ncol(bases)) {
        tab_1[i,1] = names(bases)[i]
        tab_1[i,2] = class(bases[,i])
        
    }
    return(tab_1)
}

lista.nombres(mtcars)
