<!DOCTYPE html>
<html>
<body>

<script>
// Student list
const students = [
  { name: "Alice", dob: "2005-02-20" },
  { name: "Bob", dob: "2004-02-20" }
];

// Check birthdays
function checkBirthday() {
  let t = new Date(), d = t.getDate(), m = t.getMonth()+1;

  students.forEach(s => {
    let b = new Date(s.dob);
    if (b.getDate() === d && b.getMonth()+1 === m)
      alert("🎉 Today is " + s.name + "'s Birthday!");
  });
}

// Run
checkBirthday();
</script>

</body>
</html>
