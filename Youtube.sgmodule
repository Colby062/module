#!name= Youtube
#!desc=Block Ads Youtube (IOS >= 15)

#Telegram:https://t.me/ftos_team
# > Feature
# Xóa quảng cáo và video ngắn, tìm kiếm
# Xóa quảng cáo dạng video trong Shorts
# xóa nút tải lên dưới cùng
# Thêm hình trong hình (PIP), phát lại nền (Beta)
# Thêm dịch tự động)

[Script]
youtube.request = type=http-request,pattern=^https:\/\/youtubei\.googleapis\.com\/youtubei\/v1\/(browse|next|player|reel\/reel_watch_sequence)\?,requires-body=1,max-size=-1,binary-body-mode=1,script-path=https://raw.githubusercontent.com/Maasea/sgmodule/master/Script/Youtube/dist/youtube.request.beta.js
youtube.response = type=http-response,pattern=^https:\/\/youtubei\.googleapis\.com\/youtubei\/v1\/(browse|next|player|search|reel\/reel_watch_sequence|guide|account\/get_setting)\?,requires-body=1,max-size=-1,binary-body-mode=1,script-path=https://raw.githubusercontent.com/Maasea/sgmodule/master/Script/Youtube/dist/youtube.response.beta.js

[Map Local]
^https?:\/\/[\w-]+\.googlevideo\.com\/initplayback.+&oad data="https://raw.githubusercontent.com/Maasea/sgmodule/master/Script/Youtube/dist/blank.txt" header="Content-Type: application/vnd.yt-ump"

[MITM]
hostname = %APPEND% *.googlevideo.com, youtubei.googleapis.com
