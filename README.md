# ES6 Essentials

### Promises
javascript에서는 대부분의 작업들이 비동기로 이루어집니다.
어떤 작업을 요청하면서 callback함수를 등록하면, 작업이 수행되고 난 후에
결과를 callback함수를 통해서 알려주는 방식입니다.

초기의 javascript는 특정 event가 발생했을 때, 특정 작업을 수행하는 callback함수를 호출하는 수준이었습니다.
최근에는 이 규모가 굉장히 커져서 복잡도가 증가했고,
하나의 작업을 callback으로 결과를 받은 뒤, 다음 작업을 순차적으로 진행하는데 있어서 callback의 중첩현상이 발생합니다.
이 문제를 해결하는 제안이 Promise라는 패턴입니다.

+ Promise의 장점
>비동기 작업들을 순차적으로 진행하거나, 병렬로 진행하여 컨트롤이 비교적 쉬워지고 코드의 가독성이 좋아집니다.
>또한, 내부적으로 예외처리에 대한 구조가 잘 되어 있기에 오류가 발생했을 때 보다 쉽게 발견을 가능하게 해줍니다.

+ Promise의 상태
> pending : 아직 promise를 수행 중인 상태. fullfilled와 reject가 되기 전의 상태.

> fulfilled: promise가 지켜진 상태.

> rejected: promise가 어떤 이유에서 못 지켜진 상태.

> settled: promise의 수행여부와 관련없이 일단 결론이 난 상태.

### Const / Let
자바스크립트의 변수 선언방법에는 var, let, const 이렇게 크게 3가지가 있다. 

변수선언 방법 let, const를 사용하면 상당한 이점이 있다.

우선 두 개의 공통점은 변수 재선언 불가능이다.
let은 변수에 재할당이 가능하지만,
const는 변수 재할당이 불가능하다.

### Arrow Functions

자바스크립트가 ES6로 개정되면서 새로 들어온 Arrow Function이라는 개념이다.

() => {}의 형태를 가지고 있다.

여기서는 기존의 함수에서의 this의 기능과는 달리, this는 일반적인 인자/변수와 동일하게 취급됩니다.

따라서, Arrow Function에서는 .bind method와 .call method를 사용할 수 없습니다.


### Array Methods (map, reduce, filter, slice, splice)



### Spread Operator (Array/Object Spread)

### Export / import

