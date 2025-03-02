function manyChecks() {
    let a = Math.floor(Math.random() * 20) + 1;
    console.log(`a = ${a}`);

    let result;

    // Преобразование в if...else
    if (a > 10) {
        result = 'a is bigger than 10';
    } else {
        result = 'a is less than or equal to 10 ';
        if (a === 5) {
            result += 'an example of a special case';
        }
    }

    if (a === 15) {
        result += 'but a is not 15';
    }

    if (a > 5) {
        result += 'and a is greater than 5';
    } else {
        result += 'and a is less than or equal to 5 ';
    }

    if (a % 2) {
        result += ' and a is odd';
    } else {
        result += ' and a is even ';
    }

    console.log(`Результат (if...else): ${result}`);

    // Преобразование с использованием switch (частично)
    let resultSwitch = "";

    if (a > 10) {
        resultSwitch = 'a is bigger than 10';
    } else {
        resultSwitch = 'a is less than or equal to 10 ';
        switch (a) {
            case 5:
                resultSwitch += 'an example of a special case';
                break;
        }
    }

    switch (a) {
        case 15:
            resultSwitch += 'but a is not 15';
            break;
    }
    if (a > 5) {
        resultSwitch += 'and a is greater than 5';
    } else {
        resultSwitch += 'and a is less than or equal to 5 ';
    }

    switch (a % 2) {
        case 0:
            resultSwitch += ' and a is even ';
            break;
        case 1:
            resultSwitch += ' and a is odd';
            break;
    }

    console.log(`Результат (switch): ${resultSwitch}`);

}

manyChecks();
