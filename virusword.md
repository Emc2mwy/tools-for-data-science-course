```python
import matplotlib.pyplot as plt 


def plot_resumes(plt):
    data = [ ("novel coronavirus", 100, 15), ("virus propageation simulation", 95, 25), ("covid-19 patients", 75, 50),
         ("disaster and opportunity", 50, 40), ("drinking alcohol increases the risk of infection", 80, 20), ("world health organization", 20, 60),
         ("the spread of the virus", 60, 70)]
        
    def text_size(total):
        """equals 8 if total is 0, 28 if total is 200"""
        return 8 + total / 200 * 20

    for word, job_popularity, resume_popularity in data:
        plt.text(job_popularity, resume_popularity, word,
                 ha='center', va='center',
                 size=text_size(job_popularity + resume_popularity))
    plt.xlabel("Popularity on Job Postings")
    plt.ylabel("Popularity on Resumes")
    plt.axis([0, 100, 0, 50])
    plt.show()
    

plot_resumes(plt)  
```


```python

```
