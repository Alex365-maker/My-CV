Yaroshyk Aliaksei
============

-------------------     ----------------------------
Mail:                            mralex174@gmail.com

Country and City:                Belarus. Minsk

Phone:                           +375 33 821407


-------------------     ----------------------------

About me
---------

**I strive to become the best of the best. A good and friendly team is very important to me.
Strong, purposeful, cheerful and hardworking, but sometimes lazy)
There is no work experience in companies yet. But I always try to develop and learn something new.**

1st August 2019 – Now
: **Student at Belarusian State University of Informatics and Radioelectronics** (Minsk)

     3rd year

1st September 2008 – 31st May 2019
: **Student at 26th School** (Brest)

     *Student of 26thschool. Brest. Belarus
     I was engaged in Greco Roman wrestling for 10 years Prize-winner of competitions in track
     and field, football, handball and much more.
     Participant of programming olympiads
     Candidate for Master of Sports in Greco Roman wrestling of the Republic of Belarus*

6th November 2001

    Born in Brest, Belarus

Skills
----------

**Programming languages:**

С, С++, Java, JS, HTML, CSS, MySQL, ReactJS

**Development environment**

Idea, NetBeans, Visual Studio, Visual Studio Code.

sample code
--------------------

To participate in a prize draw each one gives his/her firstname.

Each letter of a firstname has a value which is its rank in the English alphabet. A and a have rank 1, B and b rank 2 and so on.

The length of the firstname is added to the sum of these ranks hence a number som.

An array of random weights is linked to the firstnames and each som is multiplied by its corresponding weight to get what they call a winning number.

*  Task:
parameters: st a string of firstnames, we an array of weights, n a rank

return: the firstname of the participant whose rank is n (ranks are numbered from 1)

    function rank(st, we, n) {
    let max_lenght;
    let max = 0;
    let max_i = [];
  
    if(st.length == 0){
    return "No participants";
    }
     
    st = st.split(',');
  
    if(st.length < n){
    return "Not enough participants";
    }
  
    for(let i = 0; i < st.length; i++){
    
    max_lenght = 0;
    max_lenght += st[i].charCodeAt('i')-64;
    max_lenght += st[i].length;
    for(let h = 1; h < st[i].length; h++){
      max_lenght += st[i].charCodeAt(h)-96;
    }
    
    max_lenght *= we[i];
    max_i[i] = max_lenght;
    }
  
    for (let j = max_i.length - 1; j > 0; j--) {
    for (let i = 0; i < j; i++) {
      if (max_i[i] < max_i[i + 1]) {
        let temp = max_i[i];
        max_i[i] = max_i[i + 1];
        max_i[i + 1] = temp;
        temp = st[i];
        st[i] = st[i+1];
        st[i+1] = temp;
      }
    }
    }
    console.log(max_i);
    console.log(st);
    for(let i = 0; i < st.length-1; i++){
    if(max_i[i] == max_i[i+1]){
      for(let h = 0; h < st[i].length; h++){
        console.log(st[i].charCodeAt(h));
        console.log(st[i+1].charCodeAt(h));
        if(st[i+1].charCodeAt(h)-64 > st[i].charCodeAt(h)-64){break}
      if(st[i+1].charCodeAt(h)-64 < st[i].charCodeAt(h)-64){
        let temp = st[i];
      st[i] = st[i+1];
      st[i+1] = temp;
      break;
      }
    }}
    }
    console.log(max_i);
    console.log(st);
    return st[n-1];
    }


Сompleted courses
----------------------------------------

*  WayUP
*  Binary studio academy
*  OOP course at the University
*  CodeWars 45+ task
*  RsSchool

Foreign language
----------------------------------------

English language proficiency level B1. The Streamline A2/B1 course has been completed.
