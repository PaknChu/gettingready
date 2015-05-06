var str = "abca";

function numOfOccurences(str, searchStr) {
    var r = 0;
    var lastIndex = str.indexOf(searchStr);
    
    while (lastIndex != -1) {
        r++;
        lastIndex =
            str.indexOf(searchStr, lastIndex + 1);
    }
    
    return r;
}

if (numOfOccurences(str, 'a') >= 2) {
    console.log('enough a\'s!');
}
