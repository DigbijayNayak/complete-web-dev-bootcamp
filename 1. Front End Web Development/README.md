# Section 1: Front-End Web Development

# 1.6 How Does the Internet Actually Work?

- So what exactly is the Internet? A lot of people think it's a cloud, something that's hanging around in the sky.It's super complex, super difficult to understand, but actually, that's not it at all. The Internet is pretty simple. All it is is just a long piece of wire. And wire connects different computers to each other. So you might have one computer that's in London and another one that's in Seattle, and they can talk to each other and transfer data through this giant wire. Now, some of these computers attached the Internet have a very special job. They have to be online 24 seven, ready to serve you all the data and files that you are requesting when you try to access a website. And these are called servers.

- And what they do is they serve you all the data and files you need to be able to access and interact with certain websites. So these computers are called servers, and any computer that a user would use to access the Internet is called a client. Now, you can imagine a web server as a giant library that's open 24 seven, and you can go in there at any hour of the day and say, I want to see Google's home page or I want to see the latest posts on TechCrunch and would be able to serve you with all the files and data you would need to be able to view whatever website you want.

- Now, as you can imagine, if there's a library that's big enough to house all of these websites, then it's going to be pretty difficult to quickly locate the thing that you want out of this giant library. So how is this problem solved on the Internet?

- Well, let's say that you're sitting at home on your computer and you type in Google.com because you want to head over to the main Google home page. Well, what happens behind the scenes is that your browser will send that message to your ISP or your Internet service provider. So these are the people who you pay to be able to access the Internet. If you live in the US, that will be AT&T or Comcast. And if you're in the UK, that would be something like BT or TalkTalk.

- Now the message that you're sending the ISP is I want to see Google.com and the ISP will then relay that message to something called a DNS server, which stands for a domain name system server. And a DNS server is essentially just a souped up phone book. And what happens when you make that request through your browser is the DNS server will look up in its database to find the exact IP address of that website that you're trying to access.

- And every single computer that's connected to the Internet has an IP address. It's kind of like a postal code for your computer so that when people need to send and receive files on the Internet, each computer can be located and contacted using their unique IP address. And once the DNS server finds that IP address, it will send it back to your browser through the ISP, over the internet. Then you can make a direct request to that address.

- And what lives at that IP address is, of course the Google servers, and they'll be able to send you back all the files and data you need to be able to view the Google home page. Now you can try this for yourself to look up the IP address of the Google home page, head over to [nslookup.io](nslookup.io) website and type in Google.com and they should show you the exact IP address of the Google servers that you can access. So if you copy it and paste it into a new tab, then you'll be able to replicate that process and see the Google home page show up.

- So to summarize, the Internet is just a bunch of wires that connects up different computers, but it's just on a much bigger scale connecting up all the computers in the world. But what about the oceans? I hear you ask. Well, that's one of the coolest things.

- There are these massive undersea cables connecting all the continents on Earth. And if you head over to submarine cable map dot com, you can see all of these cables and see the ones that connect you up to the Internet. And these undersea cables are massive, consisting of hundreds of fiber optic fibers, each of them using lasers to transmit up to 400 gigabytes of data per second. This is a cross section of one of the cables that runs in New Zealand.

- It's an absolute marvel of modern technology, and it looks really beautiful, don't you think? And to think that every single time we load up a web page or click on a button on a website, behind the scenes was sending signals that navigates all of this crazy underwater and above water wires. And all I need is just an IP address. And through tiny electric signals, traveling at the speed of light through the oceans and halfway around the world. In a matter of milliseconds, I get to view my favorite websites, and that is how awesome the Internet is.

- And we're going to be taking it to build our own websites and web apps. And to be able to do that, we first have to understand how exactly do websites work.

# 1.7 How Do Websites Actually Work?

- how websites actually work and understand the role of the browser and the different files that it uses to render your favorite web pages. Previously on the Complete Web Development Boot Camp, you learned that the Internet consists of a wire that connects client computers with server computers, and you learn that there are special kinds of server computers called domain name service servers, which acts as a big old Yellow Pages phonebookand can look up the IP address of any website you want to access. And when you find out that IP address, you can directly hit up the server computer for the website that you want to view and they'll send you all the files and data for your browser to be able to render it on screen.

- Now, the data that you receive from that server usually consists of three types of files HTML, CSS, and JavaScript. And it's very likely that you would have come across these types of files or these words before because they're so common and they are so integral to how websites work. But what exactly do they do and why are there so many different types of files? Why can't we just have one file that's, you know, a website?

- Well, they actually have very different jobs. So, for example, the HTML code file is responsible for the content in your website. So if a website was a house, then the HTML would be the actual bricks of the house. It's the raw materials that makes up your house. Similarly, the HTML file contains the content of your website, like the text content or the images or buttons or links. The second type of files are the CSS files, and these are responsible for styling your website like the color of the walls or the shape of your door. The CSS file determines how your website will look. So what color will the background of the page be, or will the buttons have rounded corners? It targets all the content in your website that you created using HTML, for example, the text or the buttons and applies the styling to those elements. So you could use CSS to make a button red and have rounded corners and the button text to have a particular
  font. That is what CSS is for.

- Now the final component is the JavaScript code, and this is the code that allows your website to actually do things or have functionality. So if you are building a house, this would be like adding light bulbs that can turn on and off or putting in a cooker that can actually turn on a fire to heat your food. It turned your house into a home, and the JavaScript code does exactly that for a website. It turns a static website which just has pretty images or text into something that a user can actually interact with. For example, send an email in Gmail or post your breakfast on Instagram. It allows your website to actually do things and become functional, not just something pretty to look at.

- So if we take the Google home page as an example, again, once we receive these three types of files from the Google server, we can use our browser, which is a piece of software that specializes in dealing with these files. So when the browser loads up, the HTML will get to see the content of the website. So in this case, there's one image which has the Google logo. There's two buttons and there's a text box where we can enter our search term. Now when the browser then loads up the CSS files, then it will modify the appearance of those components so we don't get any extra buttons or images or anything with the CSS, But it will now look exactly the way Google wanted it to. The shape of that text box or the color of the buttons.

- And finally, using the JavaScript file, the browser gives us the functionality of this website. So we can type in a search term like Google in 1998. And by the way, you should really try this in Google because when you hit search, it'll turn Google into what it looked like in 1998. So with all these three different files, we get the content, we get the styling, and finally we get the functionality of the website. And combined together is how we create modern websites. Now, with all this knowledge that we've already acquired, we can already start messing around with real websites on the internet. So if you open up your browser and head over to Google.com, you can right click on the button, which is Google Search and click on Inspect.

- Now, what this does is it brings up the chrome developer tools. Now, Chrome has one of the best tool suites for web developers like us.

This is why at the beginning of the course, I asked you to download the Chrome browser, even if you

normally use a different browser.

So if you haven't yet downloaded Chrome, be sure to do it now before you continue.

Otherwise, some of the things that I say might not work in the coming lessons.

We're going to be exploring the Chrome developer tools in a lot more detail, but for now we're just

going to use it to do something really simple.

So you can see that Chrome Developer Tools has automatically highlighted the part of the code that's

responsible for that button that I right clicked on that I wanted to inspect.

And if we look carefully, you can see that the title of the button, which says Google search is actually

in here and we can find it right here.

Just after the word value.

And if we double click on it, then we can actually edit this title for it to say something completely

different.

So instead of Google search, let's call it Angela Search.

And then once I hit enter, you'll see that update over here.

Now, you'll notice there's also one called ARIA label Google Search.

And this is actually only for text readers rather than for our browser.

You can change that too, but it just means that you won't really see it on screen.

It's updating something that's used behind the scenes.

So be sure to double click on the correct thing.

Now, depending on what HTML content we're inspecting on the PA that we have to change might be different.

So for example, if you wanted to change the headlines on TechCrunch dot com, you can simply right

click on one of those headlines, click, inspect and find the part that corresponds to this headline,

which is right here in Black, and we can double click on it to say something completely different.

And you can actually change the front page of TechCrunch or BBC News or any website you want to.

So this is a great way of pranking your friends, especially when they can see that you're on TechCrunch

dot com and the title or any of the other pieces of text can say whatever you want it to.

And this is a great joke to play on friends who are maybe not quite as technologically advanced as you

because they haven't taken the course that you have.

Now, unfortunately, when I hit refresh on this website, you'll see that everything gets restored

to the original version of the website.

And the reason for this is because when we hit refresh, we're asking Techcrunch's servers to deliver

us the HTML, CSS and JavaScript files once again so that we can render the website on our browser.

But when we edit our website in the Chrome developer tools, effectively what we're changing is our

local version.

And this doesn't get saved when you hit refresh.

So of course then the website will update to the original content.

But in the coming lessons we're going to be working with HTML, CSS and JavaScript so that you can create

and host your own websites, live on the Internet and through learning how to code and how to build

websites.

You're going to be able to make websites that say anything you want it to look the way that you want

it to and have the functionality that you need.

So for all of that and more, I'll see you on the next lesson.

# Resources

[Download the Course Syllabus](./Web%2BDev%2BSyllabus.pdf)
[App Brewery Cornell Notes Template](./AppBreweryCornellNotesTemplate.pdf)
Submarine Cable Map
Google Chrome Browser (recommended)
Atom Text Editor (recommended)
List of Atom Plugins
VS Code Text Editor (good alternative)
VS Code Extensions
