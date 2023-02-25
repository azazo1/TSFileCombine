先下载 index.m3u8 文件
补全 index.m3u8 文件内文件的链接
用 main.py 提取 index.m3u8 文件内的所有文件链接
下载这些文件到本地
将 index.m3u8 文件中的文件连接改为本地文件路径(不用以 file:// 协议开头)
使用 ffmpeg 解码整合

# ps：用IDM从剪贴板导入可极快下载
# 播放请注意 index.m3u8 下的 key.key 文件网址
# 下载&解码 ffmpeg -protocol_whitelist concat,file,http,https,tcp,tls,crypto -allowed_extensions ALL -i index.m3u8 -c copy new.mp4
# 可以提前把ts文件下载下来，再把m3u8文件中的ts 文件网址切换成本地ts文件位置（左斜杠，不用写file://协议，直接写绝对路径）后ffmpeg解密速度才快

可能用到的工具
Internet Download Manager
FFmpeg
NotepadNext
