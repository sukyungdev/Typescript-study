# Typescript basic type

TypeScript 기본 타입.  
Type Annotation `:`을 이용해 타입 표기.

## String

```typescript
let a: string = 'A';
```

## Number

```typescript
let b: number = 10;
```

## Boolean

```typescript
let c: boolean = true;
```

## Array

```typescript
let a: [] = ['a', 'b', 'c'];
let b: Array<number> = [1, 2, 3]; // 배열의 요소가 보두 숫자일 경우
let c: number[] = [1, 2, 3]; // 배열의 요소가 보두 숫자일 경우
```

## Tuple

```typescript
let a: [string, number] = ['a', 1];
```

- 배열의 길이와 각 요소가 고정된 배열 형식.

## Enum

```typescript
enum a {
  'a',
  'b',
  'c',
}

enum b {
  a = 'a',
  b = 'b',
  c = 'c',
}
```

- 이름이 있는 상수들의 집합.
- 숫자나 문자를 할당 가능.

## Void

```typescript
function a(): void {
  console.log('A');
}
```

- 함수에서 아무것도 반환하지 않을 경우.

## Never

```typescript
function Error(): never {
  throw new Error();
}

function Loop(): never {
  while (true) {}
}
```

- 항상 오류를 출력하거나 무한루프인 함수일 경우.

## Null, Undefined

```typescript
let a: null = null;
let b: undefined = undefined;
```

## Any

```typescript
let a: any = ['a', 1, 2];
```

- 어떤 타입이든 허용하는 타입.

## Unknown

```typescript
let a: unknown = ['a', 1, 2];
```

- 어떤 타입이든 허용하는 타입.
- 문제 되는 코드를 미리 예방 가능.

## 참고자료 (reference)

[TypeScript #2 기본 타입 - 타입스크립트 강좌](https://www.youtube.com/watch?v=70w82P-KiVM&t=11s)  
[타입스크립트 기본 타입](https://joshua1988.github.io/ts/guide/basic-types.html#%ED%83%80%EC%9E%85%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8-%EA%B8%B0%EB%B3%B8-%ED%83%80%EC%9E%85)  
[The TypeScript Handbook](https://www.typescriptlang.org/ko/docs/handbook/intro.html)
[TypeScript enum을 사용하지 않는 게 좋은 이유를 Tree-shaking 관점에서 소개합니다.](https://engineering.linecorp.com/ko/blog/typescript-enum-tree-shaking/)  
[TypeScript 가이드북](https://yamoo9.gitbook.io/typescript/)  
[[TypeScript]타입스크립트 any, unknown 차이](https://developer-talk.tistory.com/198)

---

> 틀린점, 오타에 대한 것은 언제든지 알려주세요!
