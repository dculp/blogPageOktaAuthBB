<template>
  
  <div id="home">
    
    <h1 class="ui header" style="font-size: 25px;" v-if="!this.$parent.authenticated">Please Login with your BeachBody account to see the full page</h1>
    <div v-if="!this.$parent.authenticated">
      <router-link
        id="login-button"
        class="ui primary button"
        role="button"
        to="/login"
      >
      Login
      </router-link>
    </div>

    <div v-if="this.$parent.authenticated" style="color: #2c3e50;font-family: sans-serif;">
      <p style="font-size: 1.5rem;">Welcome back, {{claims.name}}!</p>
      <p>
        You have successfully authenticated against your BeachBody account, and have been redirected back to this application.  You now have an ID token and access token in local storage.
        Visit the <a href="/profile">My Profile</a> page to take a look inside the ID token.
      </p>

    </div>
  

<div style="border: 15px solid #bdc3c7;padding: 15px;font-family: source sans pro;max-width: 700px;width: 100%;margin: 20px auto;font-family: source sans pro;">
<div class="post" style="margin-bottom: 20px;">
    <div class="date" style="text-transform: uppercase;color: #3498db;letter-spacing: 0.2rem;">June 6th 2019</div>

    <div class="container">
      <img src="https://s3-us-west-2.amazonaws.com/beachbody-blog/uploads/2020/05/5-Tips-for-Sticking-to-a-Healthy-Lifestyle.960.jpg" style="width:100%;margin-top: 10px;opacity: 1;display: block;height: auto;transition: .5s ease;backface-visibility: hidden;"> 
      <div class="middle" style="transition: .5s ease;opacity: 0;position: absolute;top: 50%;left: 50%;transform: translate(-50%, -50%);-ms-transform: translate(-50%, -50%);text-align: center;">
        <div class="text">Login</div>
      </div>
    </div>

    <h2 style="color: #2c3e50;font-size: 2.0rem">5 Tips for Sticking to a Healthy Lifestyle</h2>

    <p  style="border-left: 5px solid #bdc3c7;padding-left: 5px;" v-if="this.$parent.authenticated">Maintaining a healthy lifestyle doesn’t necessarily require making a slew of huge 180-degree lifestyle changes.</p>

    <p v-if="this.$parent.authenticated">In fact, with a few common sense behaviors, you can create a healthy, sustainable relationship with food and eating that can last a lifetime.</p>

    <p v-if="this.$parent.authenticated">Here are five easy tips to get (and keep!) you on-track.</p>

    <p v-if="this.$parent.authenticated" style="font-size: 1.5rem; font-weight: bold;">1. Put Your Goal On the Calendar</p>

    <p v-if="this.$parent.authenticated">Setting timely and specific goals is one of the most effective tips to stay committed to a healthy lifestyle.</p>

    <p v-if="this.$parent.authenticated">When it comes to weight loss, people tend to set open-ended goals like, “I want to lose 10 pounds… eventually.”</p>

    <p v-if="this.$parent.authenticated">But when faced with a plate of chocolate cookies at work, having such a general goal makes it too easy to say, “Ehh, it’s okay, I can just eat a couple.”</p>

    <p v-if="this.$parent.authenticated">So, if your goal is to lose 10 pounds, then set a specific end date to help you stay on-track whenever temptations or cravings hit.</p>

    <p v-if="this.$parent.authenticated">Keeping an eye on that short-term goal will help you stay focused so you can say, “I really don’t need cookies right now.”</p>

    <p v-if="this.$parent.authenticated" style="font-size: 1.5rem; font-weight: bold;">2. Make a Realistic Plan</p>

    <p v-if="this.$parent.authenticated">Once you decide on a goal and get it on the calendar, it’s easy to get a little too ambitious and set unrealistic guidelines like, “I’ll stop eating out, meal prep every week, and eat healthy, nutritious meals ALL THE TIME.”</p>

    <p v-if="this.$parent.authenticated">All admirable things to strive for, but then guess what? Life happens.</p>

    <p v-if="this.$parent.authenticated">If you’re feeling hungry or overwhelmed, you’ll be more likely to fall off the wagon if you don’t have a realistic plan in place.</p>

    <p v-if="this.$parent.authenticated">But just because your meeting went late, or you overslept, or you didn’t have time to meal prep, doesn’t mean you can’t stick to your goal of eating healthfully.</p>

    <p v-if="this.$parent.authenticated">That’s why it’s important to create a practical, flexible plan that works for you, no matter what’s happening around you or what situation you’re in.</p>

    <p v-if="this.$parent.authenticated">Life is never consistent so you need a plan that works with your life, like 2B Mindset.</p>

    <p v-if="this.$parent.authenticated" style="font-size: 1.5rem; font-weight: bold;">3. Practice Your Plan</p>

    <p v-if="this.$parent.authenticated">Sometimes I’ll hear a client get a little too confident about their ability to control an eating situation and I’ll work with them to run through the details of their plan.</p>

    <p v-if="this.$parent.authenticated">It’s very easy to say, “I’m going to a party, but I won’t be tempted by anything. I’ll be fine.”</p>

    <p v-if="this.$parent.authenticated">While I love the confidence and enthusiasm, just thinking (or hoping!) things will be fine isn’t enough to make it true in real life.</p>

    <p v-if="this.$parent.authenticated">That’s why I help my clients walk through an event ahead of time to prepare them for when they see the pass-around appetizers and bread baskets on every table.</p>

    <p v-if="this.$parent.authenticated" style="font-size: 1.5rem; font-weight: bold;">4. Learn to Politely Pass</p>

    <p v-if="this.$parent.authenticated">A 2007 study showed people may face up to 200 “food decisions” every day!</p>

    <p v-if="this.$parent.authenticated">That sounds like a lot, but think about it: the vending machines at work, candies in the checkout line, donuts in the breakroom, the tempting choice of sides that come with lunch, your kids’ leftovers — the list goes on and on. (And on.)</p>

    <p v-if="this.$parent.authenticated">The daily parade of food can be endless and can really hinder your ability to stay consistent.</p>

    <p v-if="this.$parent.authenticated">That’s why it’s helpful to use what I call the DINTEO strategy, or asking yourself: “Do I Need This Eating Opportunity?”</p>
    <p v-if="this.$parent.authenticated">Asking yourself this question before you reach for that bag of chips gives you the opportunity to figure out whether or not you really want to have it.</p>

    <p v-if="this.$parent.authenticated">And if you’re at a party or eating out and you decide you don’t need to eat that appetizer, you can use my mom’s great line: “No, thanks — I’m good.”</p>

    <p v-if="this.$parent.authenticated">I love this phrase because “no, thanks” is quick and polite while “I’m good” provides a sense of control and a reminder to yourself that you are good without the food being offered.</p>

    <p v-if="this.$parent.authenticated" style="font-size: 1.5rem; font-weight: bold;">5. Stay Accountable</p>

    <p v-if="this.$parent.authenticated">Accountability is everything because in those moments of weakness, you’ll want a reminder of how important it is to stay on-track.</p>

    <p v-if="this.$parent.authenticated">Accountability can come in many forms. For instance, if you’re in the habit of tracking your food, you may not want that second helping if you know you need to write it down.</p>

    <p v-if="this.$parent.authenticated">It’s a great idea to seek someone to help you as well. My clients love the added sense of accountability I can provide them, which is why I created the 2B Mindset Certification program.</p>

    <p v-if="this.$parent.authenticated">Right now, there are more than 5,000 people who have signed up to be certified 2B Mindset Mentors and help people achieve more success on their sustainable weight-loss journey.</p>

    <p v-if="this.$parent.authenticated" style="font-size: 1.5rem; font-weight: bold;">The Bottom Line</p>

    <p v-if="this.$parent.authenticated">Set yourself up for success by taking simple steps to support all the hard work you’re doing to get fit and healthy for life!</p>

    <div v-if="this.$parent.authenticated">
      <p style="font-weight: bold; font-size: 1.2rem;color: #3498db;text-transform: uppercase;margin-top: 20px;">Comments:</p> <input type="text" name="comment-section" style="width: 100%; height: 100px;">
    </div>
    
    <hr style="border: 0;height: 1px;background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.75), rgba(0, 0, 0, 0));margin-top: 20px;">

  </div>

  

  <div class="post" style="margin-bottom: 20px;">
    <div class="date" style="text-transform: uppercase;color: #3498db;letter-spacing: 0.2rem;">June 5th 2019</div>

    <div class="container">
      <img src="https://s3-us-west-2.amazonaws.com/beachbody-blog/uploads/2020/03/PF-v-UPF.960.v2.jpg" style="width:100%;margin-top: 10px;opacity: 1;display: block;height: auto;transition: .5s ease;backface-visibility: hidden;"> 
      <div class="middle" style="transition: .5s ease;opacity: 0;position: absolute;top: 50%;left: 50%;transform: translate(-50%, -50%);-ms-transform: translate(-50%, -50%);text-align: center;">
        <div class="text">Login</div>
      </div>
    </div>
    
    <h2 style="color: #2c3e50;font-size: 2.0rem">Portion Fix vs. Ultimate Portion Fix: What's the Difference?</h2>

    <p style="border-left: 5px solid #bdc3c7;padding-left: 5px;" v-if="this.$parent.authenticated">If you’re an Autumn Calabrese fan, a Portion Fix follower, or if you’ve ever done a Beachbody On Demand program, you know those 7 color-coded portion-control containers are #LIFE.</p>

    <p v-if="this.$parent.authenticated">And by now, you’ve probably heard about the new Ultimate Portion Fix nutrition program. </p>

    <p v-if="this.$parent.authenticated">But you’re probably asking, “What’s the difference between Portion Fix and Ultimate Portion Fix?”</p> 

    <p v-if="this.$parent.authenticated">Portion Fix* gave you the basic tools to master portion control; Ultimate Portion Fix is a 30-day nutrition program with shopping tips, meal preps, tracking tools, hundreds of recipes, and more.</p>

    <p v-if="this.$parent.authenticated">Think of it like this: Ultimate Portion Fix expands on the foundation set by Portion Fix and takes it to the next level with more nutrition information, more support, and more options.</p>

    <p v-if="this.$parent.authenticated">Autumn has refined and clarified her portion-control approach to teach you and your family — including your kids! — how to eat delicious, healthy portions for good.</p>

    <p v-if="this.$parent.authenticated">Check out this handy chart below for a quick comparison:</p>

    <img v-if="this.$parent.authenticated" src="https://s3-us-west-2.amazonaws.com/beachbody-blog/uploads/2020/03/Portion-Fix-v-Ultimate-Portion-Fix.PIN_.jpg" style="width: 100%;">

    <p v-if="this.$parent.authenticated">And that’s just the beginning — you can read more about everything you get with the Ultimate Portion Fix here.</p>

    <p v-if="this.$parent.authenticated">Bottom line: Ultimate Portion Fix is a nutrition program that can help you gain a deeper understanding of nutrition and what it means to eat healthy.</p>

    <p v-if="this.$parent.authenticated">With the information, strategies, and healthy hacks that Ultimate Portion Fix provides, you’ll be able to create a healthy way for you and your family to eat for life.</p>

    <div v-if="this.$parent.authenticated">
      <p style="font-weight: bold; font-size: 1.2rem;color: #3498db;text-transform: uppercase;margin">Comments:</p> <input type="text" name="comment-section" style="width: 100%; height: 100px;">
    </div>

    <hr style="border: 0;height: 1px;background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.75), rgba(0, 0, 0, 0));margin-top: 20px;">
    
  </div>
  </div>

</div>


</template>

<script>
export default {
  name: 'home',
  data: function () {
    return {
      claims: ''
    }
  },
  created () { this.setup() },
  methods: {
    async setup () {
      this.claims = await this.$auth.getUser()
    }
  }
}
</script>




