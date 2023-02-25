    # ps：用IDM从剪贴板导入可极快下载
    # 播放请注意 index.m3u8 下的 key.key 文件网址
    # 下载&解码 ffmpeg -protocol_whitelist concat,file,http,https,tcp,tls,crypto -allowed_extensions ALL -i index.m3u8 -c copy new.mp4
    # 可以提前把ts文件下载下来，再把m3u8文件中的ts 文件网址切换成本地ts文件位置（左斜杠，不用写file://协议，直接写绝对路径）后ffmpeg解密速度才快
