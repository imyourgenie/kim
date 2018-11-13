import requests
r=requests.get('https://___________') #주소
r.encoding='utf8'
data=str(r.text)
begin=data.find('_____
end=data.rfind('_______
data=data[begin:end]
data=data.replace('</p>',' ')
words=data.split()

dict1={}
for w in words:
    if w in dict1:
        dict1[w]+=1
    else:
        dict1[w]=1
   #requests를 이용해 불러온 웹사이트에서 불필요한 정보 삭제하고, 원하는 정보만 저장한 뒤 Flask 이용
