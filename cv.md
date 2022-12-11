# Asya Kandan

## Contacts
* **Location**: Elista, Russia
* **Email**: asyakandan@gmail.com
* **Telegram**: @asyakandan
* **Github**: [asyakandan](https://github.com/asyakandan)

## About me
I'm 29 years old. I worked in Russian Agricultural Bank. Extremely motivated for career change goal. I learn Front-end development.

## Skills
* Python 3 basics
* SQLite basics
* HTML 5, CSS 3 / Sass / SCSS
* BEM-naming
* JavaScript basics
* Git, GitKraken

## Code example
[Persistent Bugger](https://www.codewars.com/kata/55bf01e5a717a0d57e0000ec): Write a function, persistence, that takes in a positive parameter num and returns its multiplicative persistence, which is the number of times you must multiply the digits in num until you reach a single digit.

```
function persistence(num) {
	let str = '' + num;
	let counter = 0;

	while (str.length != 1) {
		let result = 1;
		counter++;

		for (let el of str) {
			result *= el;
		}

		result = '' + result;

		[str, result] = [result, str];
	}

	return counter;
}
```