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


#### Experience :briefcase:	

* <a href="https://github.com/Teona-tech/UnilabPythonDevelopment">Unilab Python Development Course (tasks)</a>
* <a href="https://github.com/Teona-tech/html-and-css-practices">Html and css practices</a>
* <a href="https://github.com/Teona-tech/personal-project-html-and-css">Personal Html and css project </a>
* <a href="https://github.com/Teona-tech/Personal-Project-SCSS">Personal-SCSS-Project</a>
* <a href="https://github.com/Teona-tech/js-practises">Javascript tasks</a>
* <a href="https://github.com/Teona-tech/JS-personal-project">Javascript personal project</a>
* <a href="https://github.com/Teona-tech/typescript-personal-project">Typescript pesronal project</a>



#### Education :student:	

where? | what?
 ------------ | -------------
<a href="http://www.geolab.edu.ge/"><img width=50px src="https://scontent.ftbs5-2.fna.fbcdn.net/v/t1.6435-9/145567197_2583997071890575_6494526563535501235_n.jpg?_nc_cat=109&ccb=1-3&_nc_sid=09cbfe&_nc_ohc=lDD7pKTJQJMAX-LW80Z&_nc_ht=scontent.ftbs5-2.fna&oh=d6d663a7e8c0c17bd6df1d3f226c5148&oe=60E9963F"></a> | c#,Unity
<a href="https://unilab.iliauni.edu.ge/"><img width=50px src="https://scontent.ftbs5-2.fna.fbcdn.net/v/t1.6435-9/82785721_103798394508081_1561838589170417664_n.png?_nc_cat=110&ccb=1-3&_nc_sid=09cbfe&_nc_ohc=yjwZkAHeJIMAX889-x_&_nc_ht=scontent.ftbs5-2.fna&oh=85425bf4e2d94885ac139c72e2448da9&oe=60EA0042"></a> | Python(Flask,NLTK)
<a href="https://btu.edu.ge/"><img width=50px src="https://scontent.ftbs5-1.fna.fbcdn.net/v/t1.6435-9/118974653_1185472291837040_8177821905411797845_n.png?_nc_cat=104&ccb=1-3&_nc_sid=09cbfe&_nc_ohc=DcNnWL05KywAX_aNhrK&_nc_ht=scontent.ftbs5-1.fna&oh=b85598ac9a771e5c63942823c447b268&oe=60EB4D38"></a> | IT student - BTU
<a href="https://www.tbcitacademy.ge/"><img width=50px src="https://scontent.ftbs5-2.fna.fbcdn.net/v/t1.6435-9/90989378_10157016848346188_4281205318840483840_n.png?_nc_cat=1&ccb=1-3&_nc_sid=09cbfe&_nc_ohc=xytbUNIzsYsAX89cFJe&_nc_ht=scontent.ftbs5-2.fna&oh=284af24052aebf662a152f3a1a174944&oe=60EB0570"></a> | Frontend Development
<a href="https://start.bitcamp.ge/"><img width=50px src="https://scontent.ftbs5-2.fna.fbcdn.net/v/t1.6435-9/122397052_388542505858688_891968229563768666_n.jpg?_nc_cat=109&_nc_rgb565=1&ccb=1-3&_nc_sid=09cbfe&_nc_ohc=2DE7XMn0_lQAX_UNW2B&tn=3CH5EK3Qe96y3Si2&_nc_ht=scontent.ftbs5-2.fna&oh=93de10ac64c0bc4485fccf936aa46b38&oe=60E9AA8A"></a> | JS basics


#### English level
B2-C1

