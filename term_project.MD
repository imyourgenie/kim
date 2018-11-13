#requests를 이용해 불러온 웹사이트에서 불필요한 정보 삭제하고, 원하는 정보만 저장한 뒤 Flask 이용
import requests
r=requests.get('_____')
r.encoding='utf8'
data=str(r.text)
begin=data.find('______')
end=data.rfind('___________')
data=data[begin:end]
data=data.replace('</p>',' ')
words=data.split()

dict1={}
for w in words:
    if w in dict1:
        dict1[w]+=1
    else:
        dict1[w]=1
