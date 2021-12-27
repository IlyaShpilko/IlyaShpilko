# ФИО: Шпилько Илья Сергеевич

### 1. Контактная информация:
- Адрес: Саратовская область, город Энгельс
- Телефон: 8 (905) 383-38-75
- @email: shpilkoilya@icloud.com
- github: https://github.com/IlyaShpilko

### 2. Желаемая должность и зарплата:
- Должность: Junior iOS Developer
- Зарплата: 40 000 рублей
- График работы: полный день
- Формат: в офисе/частично удаленный/удаленный
- К переезду: не готов

### 3. Ключевые навыки
- Xcode
- Swift
- Objective-C
- Foundation
- UIKit
- Xib
- CoreData
- MVC
- GCD
- Git
- ООП


### 4. Пример кода:
### SWIFT

    import Foundation
    
    func getNumberOfBoats(dwarfs: [Int], limit: Int) -> Int {
        var bool = false

        dwarfs.forEach {
            if $0 > limit || $0 < 0 {
                bool = true
            }
        }
        guard !bool else { return 0 }

        var count = 0
        var exit = [Int]()

        for dwarf1 in 0 ..< dwarfs.count {

            if dwarfs[dwarf1] == limit {
                exit.append(dwarf1)
                count += 1
                continue
            }

            for dwarf2 in dwarf1+1 ..< dwarfs.count {
                print(dwarfs[dwarf1], dwarfs[dwarf2])
                if dwarfs[dwarf1] + dwarfs[dwarf2] == limit && !exit.contains(dwarf1) && !exit.contains(dwarf2) {
                    exit += [dwarf1, dwarf2]
                    count += 1
                    break
                }
            }
        }

        count += dwarfs.count - exit.count

    return count
}

### 5. Обучение и Опыт:
- Crimea Digital Group - MOBILE IOS (прошел курс и имеется сертификат)
- Прошел тестирование на сайте GeekBrains (имеется сертификаты)
- Занимаюсь самообучением: по книгам RayWenderlich, Paul Hudson, Усова;

### 6. Иностранные языки:
- Английский: А2 

### 7. О себе:
Люблю программирование. Последний год изучаю программирование под iOS на языке Swift и Objective-C. Готов учится и развиваться в данном направлении.

Личные качества:
- Целеустремленный
- Коммуникабельный
- Ответственный
- Инициативный
- Мотивированный
- Быстро обучаемый
