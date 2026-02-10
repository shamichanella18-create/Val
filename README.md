<script>
  let yesSize = 18;
  let noCount = 0;

  const messages = [
    "Pleaseee 🥺",
    "But I love you nah 💔",
    "I am begging you 😭",
    "I will do ANYTHING 😩✨",
    "Okay now you are being mean 😭",
    "Please babyy 🥹",
    "ODINAKA if you don’t press YES 😤",
    "Ok bye 💀"
  ];

  function noClicked() {
    if (noCount < messages.length) {
      document.getElementById("question").innerText = messages[noCount];
    } else {
      document.getElementById("question").innerText = "JUST PRESS YES 😭💘";
    }
    noCount++;

    yesSize += 10;
    document.getElementById("yes").style.fontSize = yesSize + "px";

    const noBtn = document.getElementById("no");
    const x = Math.random() * 200 - 100;
    const y = Math.random() * 200 - 100;
    noBtn.style.transform = `translate(${x}px, ${y}px)`;
  }
</script>
