const board = document.getElementById("puzzleBoard");
const status = document.getElementById("status");

const imgUrl = "https://tse2.mm.bing.net/th/id/OIP.0m6VcTDEcEhpF3Sm3UC1HAHaHa?pid=Api";

let positions = [];

// Creează piesele puzzle-ului
function createPieces() {
  board.innerHTML = "";
  positions = [];
  let index = 0;

  for (let row = 0; row < 3; row++) {
    for (let col = 0; col < 3; col++) {
      const piece = document.createElement("div");
      piece.classList.add("piece");
      piece.style.backgroundImage = `url(${imgUrl})`;
      piece.style.backgroundPosition = `-${col * 200}px -${row * 200}px`;
      piece.dataset.correct = index;
      piece.draggable = true;

      piece.addEventListener("dragstart", dragStart);
      piece.addEventListener("dragover", dragOver);
      piece.addEventListener("drop", drop);

      board.appendChild(piece);
      positions.push(piece);
      index++;
    }
  }
}

// Amestecă piesele
function shufflePieces() {
  positions.sort(() => Math.random() - 0.5);
  positions.forEach(p => board.appendChild(p));
  status.textContent = "";
}

// Drag & Drop
let dragged = null;

function dragStart(e) {
  dragged = e.target;
}

function dragOver(e) {
  e.preventDefault();
}

function drop(e) {
  e.preventDefault();
  if (dragged && dragged !== e.target) {
    const draggedIndex = positions.indexOf(dragged);
    const targetIndex = positions.indexOf(e.target);

    // Schimbă pozițiile
    [positions[draggedIndex], positions[targetIndex]] = 
    [positions[targetIndex], positions[draggedIndex]];

    board.innerHTML = "";
    positions.forEach(p => board.appendChild(p));

    checkWin();
  }
}

// Verifică dacă puzzle-ul e rezolvat
function checkWin() {
  let correct = positions.every((p, i) => parseInt(p.dataset.correct) === i);
  if (correct) {
    status.textContent = "Bravo! Ai rezolvat puzzle-ul!";
  }
}

createPieces();
shufflePieces();
