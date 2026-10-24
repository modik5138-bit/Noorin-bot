# Noorin Coin Bot V7

## Features
- Arabic text commands: `رصيدي`, `بروفايل`, `تحويل`, `سحب`, `توب`, `إضافة`, `قيمة`, `إعدادات_السحب`, `جيف`, `بوكس`, `مساعدة`, `language`.
- Economy profile image with balance, XP progress, level and balance rank.
- Giveaway participation, then owner confirmation before prize is credited.
- Box: first valid click receives the prize immediately.
- Withdrawal requests go to a channel selected by the bot owner with `إعدادات_السحب #channel`; buttons `استلام ✅` and `الغاء ❌` DM the requester.
- Ticket commands/system removed.
- User language preference button (language preference is stored; current core command replies are mostly Arabic).

## Install / host
1. Use Node.js 20 or newer.
2. Upload these files and install dependencies with `npm install`.
3. In `config.js`, set `token` and `ownerId`.
4. In Discord Developer Portal, enable **Message Content Intent** for the bot.
5. Invite the bot with View Channels, Send Messages, Read Message History, Attach Files, Embed Links, and Use External Emojis if needed.
6. Start using `npm start`.

## Commands
- `رصيدي`
- `بروفايل`
- `تحويل @عضو 100`
- `سحب 1000 500` (Noorin amount, Credits amount)
- `توب`
- `إضافة @عضو 1m` (bot owner only)
- `قيمة 1` (bot owner only)
- `إعدادات_السحب #channel` (bot owner only)
- `جيف 1m 2` (prize, duration in minutes; admin/owner)
- `بوكس 1m` (admin/owner)
- `language` or `لغة`
- `مساعدة`

Amounts accept suffixes `k`, `m`, `b`, e.g. `1m`.

## Notes
- This is a virtual in-bot currency. It does not transfer real money, crypto, or external Credits.
- Giveaways reserve the prize from the host's balance and require owner confirmation to pay the winner. If cancelled, the reserved amount returns to the host.
- Box prize is deducted from the command user's balance and paid to the first clicker.
- Keep the bot token private.
