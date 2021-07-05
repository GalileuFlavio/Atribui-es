//função principal
fun main(){
val grade = (0..10).random()
    print(grade.getStudentStetus())
}

fun Int.getStudentStatus():String{
    println("nota $this") 
 
    return when (this){
    in 0..4 -> "Reprovado"
    in 5..7 -> "mediano"
    in 8..9 -> "Bom"
    10 -> "Exelente"
    else -> "Indefinido"
}

}
