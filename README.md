# Russia, China Scrollytelling 

## Update

1. Replace csv files inside data with updates:  
   `russia.json`
   `all_update.csv`
   `loc_correction.csv`
   `agts_rus_china.csv`
   `paax_practical_third_labelled_signatories.csv`

2. Update file names in `index.html` on line 217:
```js
  Promise.all([
    d3.json("data/russia.json"),
    d3.csv("data/all_update.csv"),
    d3.csv("data/loc_correction.csv"),
    d3.csv("data/agts_rus_china.csv"),
    d3.csv("data/paax_practical_third_labelled_signatories.csv"),
  ]).then(function (files) {
```

3. Deploy
```bash
git add .
git commit -m "message"
git push
```