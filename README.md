# yt-dl-error

ERROR: Signature extraction failed: Traceback (most recent call last):
  File "C:\Users\Omer Kural\AppData\Local\Programs\Python\Python36\lib\site-packages\youtube_dl\extractor\youtube.py", line 1210, in _decrypt_signature
    video_id, player_url, s
  File "C:\Users\Omer Kural\AppData\Local\Programs\Python\Python36\lib\site-packages\youtube_dl\extractor\youtube.py", line 1121, in _extract_signature_function
    res = self._parse_sig_js(code)
  File "C:\Users\Omer Kural\AppData\Local\Programs\Python\Python36\lib\site-packages\youtube_dl\extractor\youtube.py", line 1182, in _parse_sig_js
    jscode, 'Initial JS player signature function name', group='sig')
  File "C:\Users\Omer Kural\AppData\Local\Programs\Python\Python36\lib\site-packages\youtube_dl\extractor\common.py", line 972, in _search_regex
    raise RegexNotFoundError('Unable to extract %s' % _name)
youtube_dl.utils.RegexNotFoundError: Unable to extract Initial JS player signature function name; please report this issue on https://yt-dl.org/bug . Make sure you are using the latest version; see  https://yt-dl.org/update  on how to update. Be sure to call youtube-dl with the --verbose flag and include its complete output.
 (caused by RegexNotFoundError('Unable to extract Initial JS player signature function name; please report this issue on https://yt-dl.org/bug . Make sure you are using the latest version; see  https://yt-dl.org/update  on how to update. Be sure to call youtube-dl with the --verbose flag and include its complete output.',)); please report this issue on https://yt-dl.org/bug . Make sure you are using the latest version; see  https://yt-dl.org/update  on how to update. Be sure to call youtube-dl with the --verbose flag and include its complete output.
Ignoring exception in command play:
Traceback (most recent call last):
  File "C:\Users\Omer Kural\AppData\Local\Programs\Python\Python36\lib\site-packages\discord\ext\commands\core.py", line 61, in wrapped
    ret = await coro(*args, **kwargs)
  File "C:\Users\Omer Kural\Desktop\Ömer\Python Projects\Discord Bots\RuLe\Source\cogs\music.py", line 208, in play
    song = await SongInfo.from_ytdl(song_name, ctx.author, ctx.channel, loop=ctx.bot.loop)
  File "C:\Users\Omer Kural\Desktop\Ömer\Python Projects\Discord Bots\RuLe\Source\cogs\music.py", line 86, in from_ytdl
    info = processed_info['entries'].pop(0)
IndexError: pop from empty list

The above exception was the direct cause of the following exception:

Traceback (most recent call last):
  File "C:\Users\Omer Kural\AppData\Local\Programs\Python\Python36\lib\site-packages\discord\ext\commands\bot.py", line 896, in invoke
    await ctx.command.invoke(ctx)
  File "C:\Users\Omer Kural\AppData\Local\Programs\Python\Python36\lib\site-packages\discord\ext\commands\core.py", line 533, in invoke
    await injected(*ctx.args, **ctx.kwargs)
  File "C:\Users\Omer Kural\AppData\Local\Programs\Python\Python36\lib\site-packages\discord\ext\commands\core.py", line 70, in wrapped
    raise CommandInvokeError(e) from e
discord.ext.commands.errors.CommandInvokeError: Command raised an exception: IndexError: pop from empty list
