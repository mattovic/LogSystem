#### LogSystem
####Database structure
~~test~~  
Add 组数，年月日，但是分条记录  
返回值add 动作名+部位名+时间  
table main  

id | name | part | wight | times | created_at 
-------- | ---------- | ---------- | -------- | -------- | ----------
int | string | string | int | int | dateTime
####API
**GET**`/body/train`
Get training record(s)  
Request:  
Header:`?`
Response:  
Body:  
```

```
**POST**`/body/train`  
Add a training record
Request:  
Header:`?`  
Body:  
```
{
	"name": "Dead lift",
	"part": "back",
	"weight": 30,
	"times": 8
}
```
Parameter | Type
------------ | -------------
name | xsd:string
part | xsd:string
weight | xsd:int
times | xsd:int
Response:  
Header:`?`  
Body:  
```
{
	"name": "Dead lift",
	"part": "back",
	"weight": 30,
	"times": 8,
	"created_at": "2015-11-29 15:51:28.942323",
	"uuid": "0dca7d12-96b1-11e5-99ca-024d03c2f759"
}
```
Parameter | Type
------------ | -------------
name | xsd:string
part | xsd:string
weight | xsd:int
times | xsd:int
created_at | xsd:dataTime
uuid | xsd:string
