# -equb-oromiya-
Equb Oromiyaa - appii Equbii Afaan Oromootiin
python-telegram-bot
from telegram import Update
from telegram.ext import Application, CommandHandler, ContextTypes

TOKEN = "TOKEN_KEE"

async def start(update: Update, context: ContextTypes.DEFAULT_TYPE):
    await update.message.reply_text(
            "Baga nagaan dhuftan Equb Oromiyaa Bot!"
                )

                app = Application.builder().token(TOKEN).build()
                app.add_handler(CommandHandler("start", start))

                app.run_polling()
                