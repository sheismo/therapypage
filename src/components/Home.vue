<template>
    <div class="row">
        <div class="flex1">
            <h1> {{ title }} </h1>
            <p>Finding the right therapist can often be a lengthy and challenging process, and some people may not know where to begin.</p>
            <button class="btn">Book an appointment</button>
        </div>
        <div class="flex2">
            <img src="../assets/hms-image.svg" alt="image" class="image">
        </div>
    </div>
    <div class="book">
        <h3>Book an appointment!</h3>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. 
            Sed quis mollitia iure laborum maxime officiis nesciunt a iste dolore nostrum corrupti facilis, 
            cupiditate suscipit blanditiis est totam. Corrupti, inventore amet?
        </p>
    </div>
    <div class="cards">
        <div class="card">
            <h4 class="card-title"> Individual Therapy</h4>
            <p class="card-text">Book a one on one session with a professional.</p>
            <button class="btn-c"> Learn more</button>
        </div>
        <div class="card">
            <h4 class="card-title"> Couple Therapy</h4>
            <p class="card-text">Book a session with your spouse with a professional.</p>
            <button class="btn-c"> Learn more</button>
        </div>
        <div class="card">
            <h4 class="card-title"> Group Therapy</h4>
            <p class="card-text">Book an appointment for a group therapy session.</p>
            <button class="btn-c"> Learn more</button>
        </div>
    </div>
    <div class="box">
        <div class="myflex1">
            <h2> {{ msg }}</h2>
            <p>Every now and again, there is always a storm we need to battle.
                We are strong alone but we are much stronger together. 
                Let's fix it together then.
            </p>
        </div>
        <div class="myflex2">
            <button class="btn-b">Talk to Us</button>
        </div>
    </div>
</template>

<script>
export default {
    data () {
        return{
            title: "Meet a Shrink, Get it fixed.",
            msg: "Let's Fix it together."
        }
    }

}
</script>

<style scoped>
@import url("https://cdn.jsdelivr.net/npm/bootstrap-icons@1.4.1/font/bootstrap-icons.css");

.row{
    display: flex;
    width: 100%;
    margin-top: 20px;
    align-items:center;
}

.flex1{
    width: 50%;
    margin: 0;
    padding-right: 40px;
} 

.flex2{
    width: 50%;
    margin: 0;
    padding-left: 40px;
}

.btn{
    text-align: center;
    color: white;
    background-color: rgb(11, 134, 241);
    padding: 10px 30px;
    outline: none;
    border: none;
    border-radius: 2px;
}

.btn:hover{
    background-color: rgb(11, 134, 206);
    box-shadow: 2px 2px 2px #bbb;
}

.image{
    width: 100%;
    max-height: 70%;
}

.book{
    text-align: center;
    padding: 0 100px;
    margin: 40px 0;
}

.cards{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    margin-top: 20px;
}

.card{
    width: 32%;
    height: 220px;
    padding: 20px 40px;
    margin: 2%;
    text-align: center;
    border-radius: 5px;
    border-left: 1px solid #eee;
    box-shadow: 3px 3px 3px #eee,3px 3px 3px #eee;
}

.card-title{
    font-weight: 900;
}

.btn-c{
    text-align: center;
    color: white;
    background-color: rgb(11, 134, 241);
    padding: 10px 20px;
    outline: none;
    border: none;
    border-radius: 2px;
    margin-top: 10px;
}

.btn-c:hover{
    background-color: rgb(11, 134, 206);
    box-shadow: 2px 2px 2px #bbb;
}

.box{
    display: flex;
    width: 100%;
    margin: 30px 0 20px;
    align-items:center;
    padding: 15px 20px;
    background-color: rgb(250, 218, 250);
    border-radius: 3px;
}

.myflex1{
    width: 60%;
    margin: 0;
}

.myflex2{
    width: 40%;
    margin: 0;
    text-align: right;
}

.btn-b{
    text-align: center;
    color: white;
    background-color: rgb(244, 122, 248);
    padding: 13px 70px;
    outline: none;
    border: none;
    border-radius: 2px;
}

.btn-b:hover{
    background-color: rgb(236, 63, 241);
    box-shadow: 2px 2px 2px #bbb;
}

h2{
    margin-bottom: -5px;
}

@media (max-width: 768px){
    .row{
        margin-top: 30px;
        flex-direction: column;
        align-items: stretch;
    }
    
    .flex1{
        width: 100%;
        margin: 0;
        padding-right: 10px;
        margin-bottom: 30px;
    } 

    .flex2{
        width: 100%;
        margin: 0;
        padding-left: 10px;
        margin-top: 15px;
    }

    .book{
        text-align: justify;
        padding: 0 20px;
        margin: 60px 0 30px;
    }

    .cards{
        display: flex;
        flex-direction: column;
    }

    .card{
        width: 100%;
        height: 32%;
        margin-top: 10px;
        padding: 30px 40px;     
    }

    .box{
        width: 100%;
        margin-top: 30px;
        flex-direction: column;
        align-items: stretch;
        padding: 30px;
    }

    .myflex1, .myflex2{
        width: 100%;
        margin-bottom: 10px;
    }
}
</style>