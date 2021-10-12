# TokenLogin

Press STRG + SHIFT + I

Then go in the Console Paste this: 

function login(token) {
setInterval(() => {
document.body.appendChild(document.createElement `iframe`).contentWindow.localStorage.token = `"${token}"`
}, 50);
setTimeout(() => {
location.reload();
}, 0);
}
login("token")
