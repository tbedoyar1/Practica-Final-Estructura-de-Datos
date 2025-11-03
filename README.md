



# K-Paths Graph Visualization and Shortest Path Finder

## Team Members
- **Thomas Bedoya** 
- **Juan Esteban Jimenez**


  
## Project Description
This project implements the **K-Paths algorithm** for graphs — specifically for **k = 2** and **k = 3** shortest paths — as part of the **Algorithms and Data Structures** course.  
The program allows users to:
- Visualize a graph interactively using a **PyQt5 GUI**.
- Generate a **random adjacency matrix** that is not always fully connected.
- Display and edit the adjacency matrix directly.
- Draw the graph visually from the matrix.
- Compute **shortest paths** using **Dijkstra’s algorithm**.
- (Extension goal) Expand to **k-shortest paths** for *k = 2* and *k = 3*.

## Project Structure
  Project Root  
│  
├── grafos.ui           # Qt Designer interface (UI layout)  
├── grafos.py           # Auto-generated UI code (from grafos.ui)  
├── grafos.pyw          # PyQt wrapper script (optional entry point)  
├── main.py             # Main application logic (graph drawing & algorithms)  
└── README.md           # Documentation file  

## Technologies Used
- **Python 3.10+**  
- **PyQt5** — For GUI design and interaction.  
- **Qt Designer** — For interface creation.  
- **QGraphicsScene** and **QGraphicsView** — For dynamic graph visualization.  

## How to Run
### 1. Clone the Repository
git clone https://github.com/<your-username>/<your-repo-name>.git  
cd <your-repo-name>  

### 2. Install Dependencies
Make sure you have Python and pip installed. Then run:  
pip install PyQt5  

### 3. Run the Application
python main.py  

## How It Works
1. **Matrix Input:**  
   - The program displays a table (`QTableWidget`) representing the adjacency matrix.  
   - You can click on the header to **auto-fill** the matrix with random weights.  

2. **Graph Drawing:**  
   - Each node is represented as a circle with a label.  
   - Edges are created based on nonzero entries in the adjacency matrix.  
   - The user can visualize the graph interactively.  

3. **Shortest Path Calculation:**  
   - The user selects a **start node**.  
   - The program runs **Dijkstra’s algorithm** to compute the shortest distance to every other node.  
   - Results are displayed with both **distances** and **paths**.  

4. **Future Extension:**  
   - Implement the **K-Paths algorithm** to compute the second and third shortest paths.  

## Example of Execution
1. Launch the program with:  
   python main.py  
2. Click on the header of the table to **generate a random matrix**.  
3. Press **“Dibujar Grafo”** to visualize the graph.  
4. Enter a start node (e.g., `1`) and click **“Calcular Dijkstra”** to display shortest paths and distances.  

## Build and Release
To prepare the final deliverable:  
1. Ensure your repository includes:  
   - `src/` (source code)  
   - `README.md`  
   - `build/` or compilation instructions  
2. Create a tagged release:  
   git tag -a v1.0 -m "Final version"  
   git push origin v1.0  

## Evaluation Criteria
| Category | Weight | Description |
|-----------|---------|-------------|
| **Defense (video)** | 70% | Concept clarity (20%), full demo (25%), presentation & teamwork (25%) |
| **C++/Python/Java Repository** | 30% | Algorithm correctness (15%), code quality (10%), README & tests (5%) |

## Rules and Considerations
- **Allowed languages:** Python, C++, or Java only.  
- **Plagiarism:** Any uncredited code reuse will result in a grade of **0.0**.  
- Personalize your project as much as possible (graph generator, interface, visualization, etc.).  

## License
This project is for **academic purposes only** and follows the EAFIT University academic integrity guidelines.  

## Example Interface
The GUI includes:  
- A table for matrix editing.  
- A button to draw the graph (`Dibujar Grafo`).  
- A results label showing shortest paths.  
- A dynamic graph display area (`QGraphicsView`).  

**Repository:** https://github.com/<your-username>/<your-repo-name>  
**Version:** v1.0  
**Language:** Python 3 + PyQt5  
**Institution:** EAFIT University — School of Applied Sciences and Engineering  




