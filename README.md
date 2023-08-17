# Typescript
## что токое Typescript ? 
TypeScript — это строго типизированный язык программирования, построенный на JavaScript. Разработчики добавили в него дополнительные возможности, такие как статическая типизация, классы и модули, чтобы создавать более надежные и поддерживаемые программы.

TypeScript позволяет выявлять ошибки на этапе разработки, облегчает совместную работу в команде и улучшает производительность разработки в больших проектах. Он преобразуется в обычный JavaScript, поэтому код, написанный на TypeScript, может выполняться в любом современном браузере или окружении, поддерживающем JavaScript.

В TypeScript есть базовые типы данных 
const mynumber: number = 1
const mystring: string = "HELLO WORLD"
const myBoolean : boolean = true


Если нам нужно типизировать функцию 
function sum(a: number, b: number) (здесь пишем тип аргументов) : number ( здесь пишем возвращаемый тип функции ){
    return a + b
}

Если нам нужно создать массив 
const numbers: number[] = [1,2,3]
const strings: number[] = [a,b,c]

Пример кода на TypeScript
 type User = {
  firstName: string;
  lastName: string;
};

const formatFullName = ({ firstName, lastName }: User) => {
  return `${firstName} ${lastName}`;
};

formatFullName({ firstName: 'John', lastName: 'Doe' });

----------------------------------------------------------------------------------------


Например,
если у нас есть переменная age, мы можем указать ее тип как number, чтобы ограничить ее только числовыми значениями. Это позволяет нам избежать ошибок, например, попытку присвоить строковое значение переменной age.



#### В чем разница между TypeScript и JavaScript.

                    
   1. Типизация
В отличие от JavaScript, у TypeScript строгая, статическая типизация. Это значит, что переменные, параметры функций и другие элементы кода должны быть объявлены с указанием типа данных. Статическая типизация позволяет выявлять ошибки на этапе разработки и делает код более надежным.

Типы это множество различных значений. Типы в Typescript используется для определения данных.
Которые  могут быть использованы в программе


----------------------------------------------------------------------------------------------
Также присутствует тип any
который по сути игнорирует проверку типизациии

let a: any = "1"

a = () => 1
и в дальнейшем мы можем добавить любой тип.

Для того что бы сказать ыто мы используем 2 потонциальных типа мы используем unionType
например:
function addOne(num: number | string):number (unionType){
    return 1 + Number(num 
}

Но для того что каждый раз так не писать мы можем создать свой тип 

type numberOrstring = number | string
function addOne(num: numberOrstring):number (unionType){
    return 1 + Number(num 
}

Для того что бы написать обьект

const Person:{
    name: string
    age: number
    hobbies: string
} ={
    name: Salman,
    age: 24,
    hobbies: sport
}

НО ДЛЯ ТОГО ЧТО БЫ ЭТО БЫЛО УДОБНО МЫ МОЖЕМ ВСЕ ЭТО ПЕРЕНЕСТИ В INTERFACE

interface User{
    name: string
    age: number
    hobbies: string
} 
const User{
    name: Salman,
    age: 24,
    hobbies: sport
}
-------------------------------------------------
### Есть также специальные типы unknown
let a: unknown = 42

Если мы незнаем что это за тип в текующий мамент гл узаем позже

let b = a == 42 ? 'hello ' : "world" 


если функция не когда не заканчивается то тогда ей приобразуем : never

function infinity (): never{
    while(true){
        console.log(1+1);
    }
}


---------------------------------------------------------------------------

#TJ
### Typescript
##  Typescript чист ? 
TypeScript забони барномасозии сахт чопшуда аст, ки дар JavaScript сохта шудааст. Таҳиягарон ба он хусусиятҳои иловагӣ, аз қабили чопкунии статикӣ, синфҳо ва модулҳо илова карданд, то барои эҷоди барномаҳои мустаҳкамтар ва нигоҳдорӣ мусоидат кунанд.


TypeScript ба шумо имкон медиҳад, ки хатогиҳоро дар марҳилаи рушд дарёфт кунед, ба ҳамкории даста мусоидат мекунад ва маҳсулнокии рушдро дар лоиҳаҳои калон беҳтар мекунад. Он ба JavaScript оддӣ тарҷума мешавад, аз ин рӯ рамзи дар TypeScript навишташуда метавонад дар ҳама гуна браузер ё муҳити муосир, ки JavaScript-ро дастгирӣ мекунад, кор кунад.


агар мо тағирёбандаи синну сол дошта бошем, мо метавонем навъи онро ҳамчун рақам муайян кунем, то онро танҳо бо арзишҳои ададӣ маҳдуд созем. Ин ба мо имкон медиҳад, ки аз хатогиҳо канорагирӣ кунем, масалан кӯшиши таъин кардани арзиши сатр ба тағирёбандаи синну сол.

Баръакси JavaScript, TypeScript дорои чопкунии қавӣ ва статикӣ мебошад. Ин маънои онро дорад, ки тағирёбандаҳо, параметрҳои функсия ва дигар унсурҳои код бояд бо навъи маълумот эълон карда шаванд. Навиштани статикӣ ба шумо имкон медиҳад, ки хатогиҳоро дар марҳилаи таҳия ошкор созед ва кодро боэътимодтар мекунад.

Типхо маҷмӯи арзишҳои гуногун мебошанд. Типхо дар Typescript барои муайян кардани маълумот истифода мешаванд.
Онро дар барнома истифода бурдан мумкин аст









