# helicopter
1950558335:AAHRKsB2S3tzaNLE_nCHVyM-tOHtxVB1TKc
import tgcrypto
from pyrogram import Client, filters
from pyrogram.errors import FloodWait
from time import sleep
from pyrogram import Client, emoji, filters

app = Client(
"my_account",
api_id=2657505,
api_hash="b5ef59986f55eb35e4cc63c26d243b7c"
)

@app.on_message(filters.command("type", prefixes=".") & filters.me)
def type(_, msg):
orig_text = msg.text.split(".type", maxsplit=1)[1]
text = orig_text
tbp = "."
typing_symbol = "*"

while(tbp != orig_text): 
try: 
msg.edit(tbp + typing_symbol)


tbp = tbp + text[0]
text = text[1:]

msg.edit(tbp)

except FloodWait as e:
sleep.time(e.x)
@app.on_message(filters.command(".", prefixes="") & filters.me)
def echo(client, message):
message.reply_text(message.text)
@app.on_message(filters.command(",", prefixes="") & filters.me)
async def hello(client, message): 
await message.reply_text(f"Привет тебе от {message.from_user.first_name}") 
@app.on_message(filters.command("+", prefixes="") & filters.me)
def hello(client, message):
message.reply_text(f"Пока тебе от {message.from_user.first_name}") 
@app.on_message(filters.command("/", prefixes="") & filters.me)
def hiall(client, message):
message.reply_text(f"Всем привет")
@app.on_message(filters.command("u", prefixes="") & filters.me)
def hall(client, message):
message.reply_text(f"Кто что делает?")
@app.on_message(filters.command("k", prefixes="") & filters.me)
def hil(client, message):
message.reply_text(f"как дела?")
@app.on_message(filters.command("o", prefixes="") & filters.me)
def hl(client, message):
message.reply_text(f"Что делаешь?")
@app.on_message(filters.command("t", prefixes="") & filters.me)
def hia(client, message):
message.reply_text(f"Ясно")
@app.on_message(filters.command("e", prefixes="") & filters.me)
def iall(client, message):
message.reply_text(f"Понял")
@app.on_message(filters.command("kk", prefixes="") & filters.me)
def il(client, message):
message.reply_text(f"Конечно")
@app.on_message(filters.command("w", prefixes="") & filters.me)
def l(client, message):
message.reply_text(f"Ага")
@app.on_message(filters.command("m", prefixes="") & filters.me)
def ll(client, message):
message.reply_text(f"А ты?")
@app.on_message(filters.command("i", prefixes="") & filters.me)
def qall(client, message):
message.reply_text(f"Отлично")
@app.on_message(filters.command("s", prefixes="") & filters.me)
def iall(client, message):
message.reply_text(f"Сижу")
@app.on_message(filters.command("l", prefixes="") & filters.me)
def hall(client, message):
message.reply_text(f"Лежу")
@app.on_message(filters.command("y", prefixes="") & filters.me)
def hilall(client, message):
message.reply_text(f"Ничего")
@app.on_message(filters.command("n", prefixes="") & filters.me)
def no(client, message):
message.reply_text(f"Нет")
@app.on_message(filters.command("g", prefixes="") & filters.me)
def yes(client, message):
message.reply_text(f"Да")
@app.on_message(filters.command("c", prefixes="") & filters.me)
def ok(client, message):
message.reply_text(f"Я согласен")
@app.on_message(filters.command("v", prefixes="") & filters.me)
def vou(client, message):
message.reply_text(f"Вау,круто")
@app.on_message(filters.command("tt", prefixes="") & filters.me)
def o(client, message):
message.reply_text(f"Я рад за тебя")
@app.on_message(filters.command("mm", prefixes="") & filters.me)
def ook(client, message):
message.reply_text(f"Молодец")
@app.on_message(filters.command("yx", prefixes="") & filters.me)
def k(client, message):
message.reply_text(f"ух ты!")
@app.on_message(filters.command("sh", prefixes="") & filters.me)
def pl(client, message):
message.reply_text(f"Шутка дня:Сиамские Близнецы пришли на веверинку и решили оторваться")
@app.on_message(filters.command("ya", prefixes="") & filters.me)
def oik(client, message):
message.reply_text(f"Я UserBot Созданный @NewsAutumn")
@app.on_message(filters.command("ho", prefixes="") & filters.me)
def oek(client, message):
message.reply_text(f"Хочешь фокус?")
@app.on_message(filters.command("ll", prefixes="") & filters.me)
def ll(client, message):
message.reply_text(f"А я Фильм смотрел с Мойм разработчиком")
@app.on_message(filters.command("yy", prefixes="") & filters.me)
def yy(client, message):
message.reply_text(f"Что?")
@app.on_message(filters.command("zz", prefixes="") & filters.me)
def kak(client, message):
message.reply_text(f"Как?")
@app.on_message(filters.command("ch", prefixes="") & filters.me)
def poch(client, message):
message.reply_text(f"Почему?")
@app.on_message(filters.command("za", prefixes="") & filters.me)
def ch(client, message):
message.reply_text(f"Зачем?")
@app.on_message(filters.command("mu", prefixes="") & filters.me)
def um(client, message):
message.reply_text(f"Я Корова")
@app.on_message(filters.command("sp", prefixes="") & filters.me)
def sp(client, message):
message.reply_text(f"Спокойной ночи тебе от {message.from_user.first_name}")
@app.on_message(filters.command("dy", prefixes="") & filters.me)
def dy(client, message):
message.reply_text(f"Доброе утро тебе от {message.from_user.first_name}")
@app.on_message(filters.command("dr", prefixes="") & filters.me)
def cdr(client, message):
message.reply_text(f"Поздравляю тебя с днем рождения, желаю счастья и всего самого наилучшего, открытка от:{message.from_user.first_name}")
@app.on_message(filters.command("tuf", prefixes="") & filters.me)
def tuf(client, message):
message.reply_text(f"Ты дурачок?")
@app.on_message(filters.command("md", prefixes="") & filters.me)
def mda(client, message):
message.reply_text(f"Мда")
@app.on_message(filters.command("pr", prefixes="") & filters.me)
def pr(client, message):
message.reply_text(f"Вообще прекрасно")
@app.on_message(filters.command("kr", prefixes="") & filters.me)
def kr(client, message):
message.reply_text(f"Красиво")
@app.on_message(filters.command("slp", prefixes="") & filters.me)
def sleep(client, message):
message.reply_text(f"Я спать пошел")
@app.on_message(filters.command("dz", prefixes="") & filters.me)
def dz(client, message):
message.reply_text(f"До завтра")
@app.on_message(filters.command("dd", prefixes="") & filters.me)
def dd(client, message):
message.reply_text(f"Как день прошел?")
@app.on_message(filters.command("vs", prefixes="") & filters.me)
def vs(client, message):
message.reply_text(f"Что весь день делал(а)")


app.run()
