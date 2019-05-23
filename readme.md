#JSON GENERATOR 

https://next.json-generator.com

##JSON CODE 
--
[
  {
    'repeat(5, 10)': {
      
     		id: {
                "$oid": "{{objectId()}}"
            },
            name: "{{firstName()}}",
            image: "https://dummyimage.com/600x100/dddddd/0011ff",
            number: "{{phone()}}",
             email(tags) {
        return `${this.name.first}.${this.name.last}@${this.company}${tags.domainZone()}`.toLowerCase();
     		 },
            "country_code": "{{integer(1, 9999)}}",
    }
  }
]
--
