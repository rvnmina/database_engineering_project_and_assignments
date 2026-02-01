
## Implementation Details
1. **Data Generation**
   - Generates N n-dimensional rectangles
   - Each rectangle is represented as:
     ```
     d1min d1max d2min d2max ... dnmin dnmax
     ```

2. **R-Tree Construction**
   - Insert-only R-Tree
   - Quadratic split algorithm used for node splitting
   - Trees are built separately for each dimension value

3. **Nearest Neighbor Search**
   - Random query point generated for each dimension
   - Distance computed between query point and rectangles
   - Number of nodes visited and time taken are recorded

4. **Performance Evaluation**
   - Average time taken (in milliseconds)
   - Average number of nodes visited
   - Results reported in tabular form as required

## Results
The final results are reported in the following format:

| Srl. No. | Number of Dimensions (n) | Average Time taken (msec) (T) | Average no. of Nodes visited (V) |
|----------|--------------------------|-------------------------------|----------------------------------|

The table is exported as:
- `RTree_Assignment_Table.csv`
- `RTree_Final_Result_Table.pdf`

## How to Run
1. Open `rtree_implementation.ipynb` in Google Colab
2. Run cells sequentially:
   - Data generation
   - R-Tree construction
   - NN query execution
   - Result table generation
3. Download the final PDF result table for submission

## Notes
- Time measurements are taken using Python high-resolution timers
- Results vary slightly due to random data and query generation
- Implementation follows standard R-Tree definitions as discussed in class

## Author
Ravindra Mina  
M.Tech (AI), IIT Kharagpur
