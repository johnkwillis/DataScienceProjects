# Thursday 7/29 - Text generation with an RNN
In class this past Thursday, we utilized a recurrent neural network (RNN) to train a model to generate text. After training the model with `shakespeare.txt` - following the steps I have elaborated on below - I was left with a model that could produce texts that closely emulated the input text file.
## ___Processing, vectorizing and predicting text___
#### In this case, the first step for generating text with an RNN is to vectorize the input script. To do this, I first utilized `preprocessing.StringLookup` to convert each token into unique character ids. In this form, the text data can be used for training; however, predictions in this format are not interpretable to humans. So, wrote another small function to decrypt the character ids that will be predicted by the model. 
## ___Building and training the model___
#### After loading and processing the script, I built a model containing three layers. The first layer maps the input characters to vectors with 256 dimensions. The second layer uses the inputs from the `Embedding` layer and processes them through a RNN with `size_units = 1024`. And finally, the third layer generates the  model's output - assigning probabilities to each possible character in `vocab`.
#### Training this model took my laptop a tremendous amount of time. Following the approach in the notebook, I used a loop to train my model - running over a total of 20 epochs. 
## ___Generating text___
#### After building and training my model, I wrote a number of functions to generate a new script (1000 characters). My final results were suprisingly coherent for such a small amount of training, however I believe there is a great deal of room for improvement. If time allows, I hope to test this script further with a model trained over more epochs. The new script my model generated (10000 characters) is below.
```
ROMEO:
So thank you for your brother without a tongue
Unto his violence, which to last
The bloty of the day,
methink you ungentle wrong, yet here on her
curst the moving affright my captieve thee:
Had live an appoue were torance? Hent thou art,
Simpling drews, which touch this news:
But sit in thinkest all receivishmonds:
Thick how we are stay, and his holy and
Clifford let me know not whether I was moved. Think,
I will be written; fly, if we bleased as thou art,
Like that vistress drop with brother's lights,
Will have the fire go go! Give mean a weary-blown as she
comes heart, divorce, to make them from them coult what my die
In to a huncrusy pleadest of reasons.
KING RICHARD II:
Such great duty; let us be consul.
ROMEO:
O word more for this! past on, gove this very goes,
First, this tail I please; men are to see thee artrows.
EXTON:
Why, what's the thiar, maste, must be fit up by,
Beshrew'd their pierces. But in true please.
You're poor mouth, the father of our kingdom shall
We two wind should not.
Here's none return, sir.'
Boy! his love, might be so heel-best, adieu;
My smile upon my custom; for you will find me
Tubsting, hast thou banish'd from the world:
And impire it in my soul and sweet
Good, for our entertain and honour dotch his
mistrusting isle and curst and loud
use: it is: I think my most abtraction.
BIPAM:
In life he was makes Petruchio.
with neither burn'd and heart fruiting breach;
Buck lowly deliver away.
LADTES:
Ay, she shall be their jest was rich and lamp's no portance,
So soundly the botodg: you first thou here,
Our garlen pleasons which was prince, my wife,
And speak a breach-off! a beast
could speak: you mistress
Stand upon the thought behild by boy-sorced round,
It once hid A hitting thing in my troblet
with deed; for thou art accused the face.
PROSPERO:
The kingdom was even, for the augher-clance
And praise yet in my husband's lands,
My master earthly passed with him, beseech
your further stone, let me all keeped by him.
DUKE OF YORK:
Thy shepherd to the gods, for they do him were, while we here
thy desert. Sharl it were as, thou in a house of yours
In spend at a pertition,--
With my beshem and my heart-too, I'ld night;
A calmai' when the suns thereof voices:
The repal themselves
With one as to all but 'tis boldly good!
In easy, being richer and proud comes creature
His father's children: pass to thee.
YORK:
Past anqweet since: hence, in door one,
I lay fight, for I canst do so: blesh you were discline,
And, my dear carces sleep; but I would be
prained and purpe and your mind and his fove,
Where he who hath order dropping to my swift so blindly,
Having no fight as big at Speak.
Provost:
I think, beggar with when this noble mulliance
From such a kind of noble duke,
And visit haths to thee to them, to the
burward, makes the joather called them of your wonder
Were at the abulments. Show your lady doth he hath
ever in thy day: in every discrept,
And will unto thy father's point.
KING RICHARD II:
You do forso thy unrest you.
LUCENTIO:
Sir, he had been
Disburk to die to the king and loves.
BUCKINGHAM:
Madam, it does not.
LARTIUS:
Leconful milshes, is all abroach
Hathard
But that she shall be well knowledge;
And, if I cannot, with all their hearts for the bowel best;
for you for your mistress frowning to A cholerance,
Alack, all of night nor days of made
Sip blows to see 'cain he with his wife's crown,
As I thou stand'st nobour of this princely called
Nothing weep.
Well, believe, sir, I hap advised and clouded fled;
Like, and just possessed it for poor.
Who asks mischief they live, to Back, wife,
And I will give a marvell an nothing but their fure
Weeping, must be wine and quiet wide and farm
That oft
With the desiress of last tame.
GREMIO:
Kate: but what, brave more would tell me, I have soon-used wither'd
Against the rock, thou art forbid'd back
to vision with thee stusin's friend.
KING RICHARD II:
Why but the tuborrow us and presently,
As many way unknown boldness. What thy durst knot I chole
beloughting her too anone. Well for her cliff, master cliff,
Will do thee knave to tell thee this.
WARWICK:
Peace, what any of her corofations shouds,
To say the time which are my will give me
These restority should dost thit,
Shook home to use the stroking-else, Edward's.
What dost thou bid it up.
GRUMIO:
O blind home, sir. I think 'tis commits to the book.
KING RICHARD II:
Marry, look, and let love Potranot.
BUCKINGHAM:
Make harm yourself flow, of them not, my brother 's.
QUEEN MARGARET:
Why, here's me love, tell me on more of our woes,
Repayed King Richard, no wormon wining better;
Our doth beget of what I promise,
LUCIO:
I have show him.
Provost:
I do enough the battle well: he is in voice in,
And, make and old amoo the door.
JULIET:
What's thy firm, he's Beasts? for they lie.
HORTENSIO:
Many liege, Sistician: but, for Pouling faced!
But whereon I shall be wondrous; I
have helps from the better to the law.
Nurse:
You should be gone-son? while, some oath
The hand-hends, cry 'good delig it betwime the older
hand of dim'd fires; and as a queen,
For marmphank my husband, when at all-times
As you are dull stone and court her.
NORTHUMBERLAND:
Nay, let me think and joy hath hell adventius here;
You said 'tis weep. Now, say the house unto the king's,
When he requires their blood is mile,
Who starved store but this world call I bled.
The world they for you three-tongue to fight,
Unlaw him blessed here, thoufand, I cannot cast him ble.
A bow duples, Warwick fits the fresh women, if thou darest us
to him.
AUFIDIUS:
Why aven too long waved. My double, I would have still they for.
PAULINA:
Will have you speak?
BAPTISTA:
Wilt thou wilt be more importune till.
QUEEN MARGARET:
Think down with some before I have been wink
Would they do great ammility to make your face,
As I may lose your fortune or their five:
Therefore hold entle is a mad--done.
ROMEO:
And I am glad,'
'Twas thou the vilu born to be forspointed
The violets are flamediance, and lets guess
From years of the broken blood to them
And aspident up his head. Ah, what I here?
KING EDWARD IV:
Northumberland, and I not pentle:
Give me asbition: ce, O'f the thoughts of Marset,
As if we see the fasting end:
Hear noices.
MARCIUS:
Over and as hast they honest.
ROMEO:
What, do I have no man maid your lobing lime and
will discreate. Hence! whree--
I'll put you you. I have safempted from his frinn and soon,
'twere the stubbornglable. Rivers, and let them not
To satity and my soldiers is the vows
Chequet my ease. But suffer, let them be.
Poot:
He came weep in God's affair.
JULIET:
Hie to her what we charnel him, and for the prince.
RIVERS:
Or spritolity furm, thou art done close,
I am for well do him in hand.
DUKE OF CARLISBY:
Me heavens and brok, he was here both: you would
ne'er back the tomb: make him and in my hands and waims
Time to retire: if the dark of great further mark,
Subution to the affairs. Take me all tubles with a
promise; the world cupas of thy breast,
As they poop-cious for hour to make you.
YORK:
Marqual king, if you delia, to-night:
And forba despair.
KING RICHARD II:
Rame to't, thou stift cheer man. Why do you dishing it for.
The glass Is courtesy, in a hole althora
And id his grant and presence toblied.
LUCENTIO:
O'er the sea begins contented:
The thender grows shall be fetting: but march leave weed.
Sir, so I think it is how? This is well:
nerry thou to at all with her.
Swirt an old-master!
LICENTIA:
On I, sirrah!
TRANIO:
Let me amblound with her, your mistress! Look back the shepherd
Hang on him.
Lord Murderer:
Call him, either muster methough to do the ground
Mishoubt, to seek me for a chole till I came.
ROMEO:
It is in this rare arm entreaty.
If I do are my leave to be done, if it be not
KING RICHARD II:
No, that I be gone! ghe meet off her?
PAULINA:
Good first, help, help! Romeo is no caff!
SAMPSON:
No,, sir, how is my health, they have been, our stin
Than feed all one. Besorall not
Show'd to living with his free any thing.
DUKE VINCENTIO:
He shew for this: after a lobie cares with a treasure
hath reposers to she should.
PROSPERO:
Now, then after many-chains,
Myself which properess; though it be so as they are.
MISTARET:
Strengthen up, and leave me, and I
will have her brother and his glory.
Come, come, lest our fore at polity,
That which have as his wife, your fish is speed,
Is very fire uneven nor protect tauthous,
I saw away their unchequence and ask
and giddy vusit, sweet sire, if he flank:
Mean to most three, and clusterness or dost, both on't;
And stoped the world and virtuoo sufferance,
Commute but menance that thou disselves
with Christian stir up. Here's the kites
With what you do cup act offended the wearyship
To access in the world--what I fear imprison'd
Here in't confess with him. Thou yours for eyes as you have ask'd,
And see, to dispenget by their tent
In oaths, sent perfent by such as for my heart?
In somitico a compass, Lucentio; hear
me and the signior Buckingham of March,
There mount about him while a king on him.
FLORIZEL:
Preporter cries 'Thou dost not place with her.
FLORIZEL:
Pray you! is it, sir! the poor words: he bot my cheek,
They all and being reprieddance to stood
To beg of thee, brother, to accident for his sibtle,
That she shall procued my climorous show a little bast
Against his eyilbue of my presermance;
Hence with the first relower and forsworn.
So back ye, I had rather give him here,
And given no pardon to simple me of you think.
Thine owe unwillingness shows; affords they that fled:
Thou setidation is more modestimal and
one ten time of all mows; or it is
coundeth a scougghen revenge for tents
That singerates become the vantage of the world,
As doitless sufferance, brother creet,
To the profit thereof and fools with old reproaf.
BUCKINGHAM:
Thou sheet, sir, an agbicion gave. Why, what would estable he?
LUCENTIO:
O hateful charts, he will now, since they
Had call'd in postet-a knee bread and beast
And hit my words. What it will not, whereford, for this m
```
