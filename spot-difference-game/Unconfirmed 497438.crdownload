let found = new Set();
const total = 8;
const counter = document.getElementById("counter");

document.querySelectorAll(".spot").forEach(spot => {
  spot.addEventListener("click", () => {
    const id = spot.dataset.id;

    if (!found.has(id)) {
      found.add(id);
      spot.classList.add("found");
      counter.textContent = `Found: ${found.size} / ${total}`;

      if (found.size === total) {
        localStorage.setItem("gameCompleted", "true");
        setTimeout(() => {
          window.location.href = "https://docs.google.com/forms/d/e/1FAIpQLSfIUO4UTqcGGs_IKwBUu7CRCjXGr6dt3uTGl4-EbUlT5j1JFg/viewform?usp=publish-editor";
        }, 1000);
      }
    }
  });
});
