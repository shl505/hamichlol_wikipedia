# hamichlol_wikipedia
סקריפט להתקנה בסימניה בדפדפן למעבר מערך באתר המכלול לערך המקביל באתר ויקיפדיה העברית
## הפעלה
כדי להפעיל את הסקריפט צרו סימניה בדפדפן והפניסו בה במקום כתובת אינטרנט את הקוד הבא:
```js
javascript:
tex=location.href;
if (tex.includes("hamichlol")){
  if (tex.includes("w/index.php")){
    {tex2=tex.replace('www.hamichlol.org.il', 'he.wikipedia.org')}
  }
  else {
    {tex2=tex.replace('www.hamichlol.org.il', 'he.wikipedia.org/wiki'); }
  }location=(tex2)                  }

else if (tex.includes("he.wikipedia")){
  if (tex.includes("w/index.php")){
    {tex2=tex.replace('he.wikipedia.org', 'www.hamichlol.org.il')}
  }
  else {
    {tex2=tex.replace("he.wikipedia.org/wiki", 'www.hamichlol.org.il'); }
  }location=(tex2)                  }

else if (tex.includes('commons.wikimedia.org/wiki/File:')){
  {tex2=tex.replace('commons.wikimedia.org/wiki/File:', 'www.hamichlol.org.il/קובץ:'); }
location=(tex2)                  }

else {alert ('הסקריפט אינו מיועד לאתר זה או לעמוד זה')}
```

וכשתרצו ל עבור מהאתר ויקיפדיה לאתר המכלול או להפך פשוט לחצו על הסימניה
