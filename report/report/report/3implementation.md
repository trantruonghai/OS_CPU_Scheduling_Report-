## Gantt Chart Implementation

```python
import matplotlib.pyplot as plt

def draw_gantt(gantt_data):
    for process, start, end in gantt_data:
        plt.barh(process, end - start, left=start)

    plt.xlabel("Time")
    plt.ylabel("Process")
    plt.title("Gantt Chart")
    plt.show()
```

