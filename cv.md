# Teona Porchkhidze :rocket::nerd_face:
##### Junior Frontend Developer

 
 <img src="https://i.ibb.co/qMQcvfZ/te-1.png"> | Hello, I am Teona, 20 years old, Startuper and Junior Frontend Developer, who has passion to study programming and use it in a creative way...
 ------------ | -------------
## my goals in 2021-2022 🔥🔥🔥
* Teona as a Full Stack Developer in EPAM :computer:	
* Success - <a href="https://www.facebook.com/300tsavleblo">300წავლებლო :yellow_circle: 300tsavleblo </a> (it's educational startup) :raised_hands:
* Winning Grace Hopper award :trophy:


#### Contact me :handshake:	

* <a href="https://www.facebook.com/teona.porchkhidze.7545/">Facebook</a>
* <a href="https://www.linkedin.com/in/teona-porchkhidze-b757b81b3/">LinkedIn</a>

#### Skills :dart:

<div align="center">
<img width=50px src="https://scontent.ftbs5-1.fna.fbcdn.net/v/t31.18172-8/15676033_895560890581516_6410598526344675319_o.png?_nc_cat=104&_nc_rgb565=1&ccb=1-3&_nc_sid=09cbfe&_nc_ohc=e_Aan2v0SyMAX9qbuIH&_nc_ht=scontent.ftbs5-1.fna&oh=1bd7f065f7280f798354f8c49e606679&oe=60EB3B4E">
<img width=50px src="https://scontent.ftbs5-1.fna.fbcdn.net/v/t1.6435-9/69316430_105309520840908_7886975276029050880_n.png?_nc_cat=104&ccb=1-3&_nc_sid=09cbfe&_nc_ohc=eG_YCwF-u8oAX84UH5B&tn=3CH5EK3Qe96y3Si2&_nc_ht=scontent.ftbs5-1.fna&oh=6a091931ea73ee41ffd8400e6d2844b9&oe=60EAFE3B">
<img width=75px src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/10/CSS3_and_HTML5_logos_and_wordmarks.svg/1280px-CSS3_and_HTML5_logos_and_wordmarks.svg.png">
<img width=50px src="https://scontent.ftbs5-2.fna.fbcdn.net/v/t1.18169-9/1010076_477783955633350_1900224762_n.png?_nc_cat=109&_nc_rgb565=1&ccb=1-3&_nc_sid=09cbfe&_nc_ohc=sYXJYwOodKUAX8eGtJN&_nc_ht=scontent.ftbs5-2.fna&oh=8d676ec43ba1e5195ba434f78f9c207f&oe=60EA1701">
<img width=67px src="https://sass-lang.com/assets/img/logos/logo-b6e1ef6e.svg">
<img width=37px src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/22/Pandas_mark.svg/1200px-Pandas_mark.svg.png">
<img width=50px src="https://techscript24.com/wp-content/uploads/2020/10/86498201-a8bd8680-bd39-11ea-9d08-66b610a8dc01.png">
<img width=50px src="https://scontent.ftbs5-2.fna.fbcdn.net/v/t1.18169-9/13645265_10154396860566789_4855137813969521495_n.png?_nc_cat=111&ccb=1-3&_nc_sid=09cbfe&_nc_ohc=U2TAw4j9svkAX-ckfqi&_nc_ht=scontent.ftbs5-2.fna&oh=f0835b85b80507600a918460af5bf8ba&oe=60EA2214">
<img width=50px src="https://sunlightmedia.org/wp-content/uploads/2017/02/git_logo-1.png">
<img width=50px src="https://scontent.ftbs5-1.fna.fbcdn.net/v/t31.18172-8/13497772_1053449538059118_5470362141370549738_o.png?_nc_cat=102&ccb=1-3&_nc_sid=09cbfe&_nc_ohc=lLHXLzlcYZsAX8Wyovf&tn=3CH5EK3Qe96y3Si2&_nc_ht=scontent.ftbs5-1.fna&oh=87dbc6c604f8f8ef4a49827a1ae6f26b&oe=60EADA1F">
</div>

#### Code example :computer:	

```

class DB {
    constructor (){
       this.person = new Map();
       this.id = 0
    }
    
    create(person){
        if(typeof person !== 'object' || !person.name || !person.age || !person.salary || !person.country){
            throw new Error("blabla");
        }
        let user = this.person.set(this.id.toString(), person);
        let tempid = this.id
        this.id++;
        return tempid.toString();
        
    }
    read(id){
        if(typeof id !== 'string'){
            throw new Error ("id must be String");
        }
        else if (this.person.has(id) === false){
            return null;
        }
        else if(this.person.has(id)){
           return this.person.get(id);
      } 
    } 
    readAll(){
    if(arguments.length != 0) throw new Error('there shouldnt be any arguments')
    	let array = [];
      this.person.forEach((index)=>array.push(index));
      return array;
    }
    update(id,obj){
			if(!this.person.has(id) || typeof id != 'string' || Object.values(obj).length < 1)
      throw new Error('wrong id')
      this.person.set(id,{...this.person.get(id),...obj})
      return id;
    }
    delete(id){
    console.log(id, this.person.get(id))
    if(!this.person.has(id))throw new Error('that person doesnt exist')
    	return this.person.delete(id)
    }
}
const db = new DB();

const person1 = {
    name: 'Pitter', // required field with type string
    age: 21, // required field with type number
    country: 'ge', // required field with type string
    salary: 500 // required field with type number
};


let id1 = db.create(person1);
let id2 = db.create(person1);
let id3 = db.create(person1);
console.log(db.read(id1));
db.readAll();
db.update(id2, {age: 6});
db.update(id1, {age: 16, name: 'teo'});
db.delete(id3);
db.readAll();

```
