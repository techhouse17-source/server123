function oldBooks(input) {
    
  let index = 0;
  let favouritebook = input[index++];
  let currentbook = input[index++];
  let bookschecked = 0;

  while (currentbook !== "No More Books" && currentbook !== favouritebook) {
    bookschecked++;
    currentbook = input[index++];
  }
  if (currentbook === favouritebook) {
    console.log(`You checked ${bookschecked} books and found it.`);
  } else {
    console.log(`The book you search is not here!`);
    console.log(`You checked ${bookschecked} books.`);
  }
}