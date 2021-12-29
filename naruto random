const containerEl = document.getElementById('naruto_container');
    
getNaruto();
async function getNaruto(){
        const res = await fetch('https://api.jikan.moe/v3/search/anime?q=naruto');
        const naruto = await res.json();
        displayItems(naruto);
        console.log(naruto);
}

function displayItems(naruto){
    const narutoEl = document.createElement('div');
    narutoEl.classList.add('card');
    narutoEl.innerHTML =   `
                <div class = "">
                    <div>
                        <img src=" ${naruto.image_url}" alt="">
                     </div>

                     <div class = "card-body">
                        <h2>Title: ${naruto.title}</h2>
                        <h3>Members: ${naruto.members}</h3>
                        <p>Number of episodes: ${naruto.episodes}</p>
                        <p>Description: ${naruto.synopsis}</p>
                    </div>
                </div>`;

    containerEl.appendChild(narutoEl);

};
