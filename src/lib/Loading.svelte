<main>
    
    <h1>payverge</h1>
    
    <div class="things">
            <div class="thing">
                <div class="thing">
                    <div class="thing">
                        <div class="thing">
                            <div class="thing">
                                <div class="thing">
                                    <div class="thing">
                                        <div class="thing">
                                            <div class="thing">
                                                <div class="thing">
    
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
    </div>
</main>


<style>
    :global(*) {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

main {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  overflow: hidden;
  gap: 2rem;
  background-color: rgba(0, 0, 0, 0.943);
}

h1 {
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-size: 3rem;
    color: white;
}

.thing {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 1px;
  border: 10px solid transparent;
  border-color: tomato transparent transparent tomato;
  border-radius: 50%;
  animation: thing 5s cubic-bezier(0.35, -0.14, 0.79, 1.22) infinite;
}

@keyframes thing {
  100% {
    transform: rotateZ(1turn);
  }
}
</style>
