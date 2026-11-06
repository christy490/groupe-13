async function loadWallet() {

    try {
        const response = await fetch(
            "/api/wallet/balance"
        );

        if (!response.ok) {
            throw new Error("Impossible de charger le solde");
        }

        const data = await response.json();

        document.getElementById("balance")
            .textContent = data.balance + " FCFA";

    } catch (error) {
        console.error(error);
    }
}

function sendMoney() {
    alert("Ouverture du formulaire d'envoi");
}

function receiveMoney() {
    alert("Ouverture du formulaire de réception");
}

loadWallet();
