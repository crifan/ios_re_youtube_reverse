# 返回数据

某个广告视频的内部返回数据：

hook代码：

```c
- (void)setVideoDetails:(id)arg1{
    iosLogInfo("arg1=%@", arg1);
    %orig;
}
```

输出：

```bash
2022-03-28 20:36:41.954044+0800 YouTube[25775:2715494] hook_ youtubeDylib.xm YTWatchMiniBarViewController$setVideoDetails$: arg1=<YTIVideoDetails 0x281b27f40>: {
    video_id: "LA6szWzus0g"
    title: "Get Chrome for iOS"
    length_seconds: 30
    channel_id: "UCL8ZULXASCc1I_oaOT0NaOQ"
    is_owner_viewing: false
    short_description: "Chrome is a fast, easy to use, and secure web browser for iOS. Get Chrome now. https://apps.apple.com/us/app/google-chrome/id535886823"
    is_crawlable: false
    thumbnail {
      thumbnails {
        url: "https://i.ytimg.com/vi/LA6szWzus0g/hqdefault.jpg?sqp=-oaymwEYCHgQWkhG8quKqQMMCAEVAACIQnABwAEG&rs=AOn4CLBU26fMso0e3iR2comi4Uz-x5cj7Q"
        width: 120
        height: 90
      }
      thumbnails {
        url: "https://i.ytimg.com/vi/LA6szWzus0g/hqdefault.jpg?sqp=-oaymwEcCIACEJABSEbyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLA2zPsvsB2aQxkZvfPFXMVhwdkpHQ"
        width: 256
        height: 144
      }
      thumbnails {
        url: "https://i.ytimg.com/vi/LA6szWzus0g/hqdefault.jpg?sqp=-oaymwEcCMACELQBSEbyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLDOaI6fXD2ptZTQmDP1myZBfcg13Q"
        width: 320
        height: 180
      }
      thumbnails {
        url: "https://i.ytimg.com/vi_webp/LA6szWzus0g/hqdefault.webp"
        width: 480
        height: 360
      }
      thumbnails {
        url: "https://i.ytimg.com/vi_webp/LA6szWzus0g/sddefault.webp"
        width: 640
        height: 480
      }
      thumbnails {
        url: "https://i.ytimg.com/vi/LA6szWzus0g/hq720.jpg?sqp=-oaymwEcCK4FEIIDSEbyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLDvGWQtBtiONoEcK933xt4Aypr_7w"
        width: 686
        height: 386
      }
    }
    allow_ratings: true
    view_count: "26531222"
    author: "Google Chrome"
    is_private: false
    is_unplugged_corpus: false
    is_live_content: false
}
```
