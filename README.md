# bookface
這是一個純 css 樣式表，將臉書的版面弄的更簡潔，順便移除廣告，經由重新安排的佈局，因此命名為「書臉」。

This a CSS stylesheet for Facebook, re-making layout clean and removing ad around window, thus called "bookface."

## Usage
#### Safari

1. 開啟「偏好設定」
2. 進入「進階」分頁
3. 在「樣式表」的地方，選擇 bookface.css
4. 重新整理臉書頁面即可

#### Chrome

1. 下載擴充功能：Stylist
2. 進入 Stylist 選項
3. 選擇 "Styles"，"Add New Style"
4. domain 輸入 "facebook.com"
5. Stylesheet Text 內貼上 bookface.css 全部內容
6. 輸入自己喜歡的名稱，Save 之後即生效。

## Customize

#### Show/Hide

第 22 到 29 行的設定，可以改變側邊欄欲顯示的項目。

Line | Element id    | Title
-----|---------------|--------
\#22 | #userNav      | 使用者
\#23 | #pinnedNav    | 最愛
\#24 | #groupsNav    | 社團
\#25 | #appsNav      | 應用程式
\#26 | #listsNav     | 朋友
\#27 | #interestsNav | 興趣
\#28 | #pagesNav     | 粉絲專頁
\#29 | #eventsNav    | 活動

Comment or un-comment line to make them show/hide.

#### View only few

Or, if you only want to see only first N items in the list of each. Change style from 

	{
		display: none;
	}

to

	{
		height: 24*N px;
		overflow: hidden;
	} 
