# Insert-Element-
Insert Element in Array by using javaScript
 let data = [3, 45, 67, 23, 56, 88, 12, 34];
      let newEl = 300;
      newEl = parseInt(newEl);
      let position = 2;
      console.warn(data);
      function getElement() {
        for (i = 0; i <= data.length - 1; i++) {
          if (i >= position) {
            data[i + 1] = data[i];
            if (i === position) {
              data[i] = newEl;
            }
          }
        }
        console.warn(data);
      }
      OutPut is:
      [3, 45, 300, 67, 23, 56, 88, 12, 34]
