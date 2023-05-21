# Task17.7.3
Программа по банковским вкладам
get_deposit = float(input())
per_cent = {'ТКБ': 5.6, 'СКБ': 5.9, 'ВТБ': 4.28, 'СБЕР': 4.0}
deposit = [rate * (get_deposit / 100) for rate in per_cent.values()]
print(deposit)
money = int(input('Введите сумму вклада'))
deposit = []
for key in per_cent:
    deposit.append(per_cent[key] * money / 100)
max_deposit = max(deposit)
print(deposit)
print('Максимальная сумма,которую вы можете заработать -' + str(max_deposit))
