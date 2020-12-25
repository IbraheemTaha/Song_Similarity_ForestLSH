# Song Similarity using Forest-LSH

Song Similarity is a Python implementation of Forest-LSH to find number of similar songs within the songs set provided in the file **_songsData.csv_** .
I will add some related projects in the future, keep tuned!


## Usage

Very simple and straight forward usage. There are two parameters you can change. The number of similar songs to be found as well as the name name of the output file as follow:

```bash
  --simsongs SIMSONGS  Number of similar songs to be found, the default is 5 songs
  --output OUTPUT      The name of the output file, the default is 'similarsongs.csv'

```

## Output

The output file is **_similarsongs.csv_ by default** which contains the ID of a song as well the corresponding similar songs IDs, separated by commas. Each ID is the number of the song in the provided file **_songsData.csv_**.
 
### Output Example

For example, the first two songs has the following similar songs (simsongs is 5 by default):

```csv
ID,song1,song2,song3,song4,song5
0,93,9,78,26,13
1,52,76,,,
```
One can notice that the second song has only two similar songs. This can happen when the Forest-LSH cannot find enough similarity in shingles to consider.


## Contribution

I am very open to your questions and suggestions!
