Some thoughts on a query interface

/resource/?attribute:opt=value

/person/?customer_id:eq=1&employee_id=10

/resource/?q=customer_id:eq=10+employee_id=10

/resource/?q=customer_id:in=10,12,23

/resource/?q=customer_id:eq=10|type:eq=10

/resource/?query=customer_id:in=10,11,12|(customer_id:eq=15+type:eq=1)&limit=15

/resource/?where=customer_id:eq=10+level:gt=5&limit=5&group=level_id

qarel
qsarel
arel search
rails search
active-record-search

Lou.parse_params()

lou = Lou.new(Person)
lou.parse(params)

lou = Lou::Base.new(Person).parse(params)

result = Lou.new(Person).parse(params)

result = Lou.parse(Person, params)

res = Lou.query(Person, params)
