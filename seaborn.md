---
title: seaborn
category: Python
layout: 2017/sheet
updated: 2020-5-9
tags: [Featured]
---

### Statistical Data Visualization With Seaborn

    ```py
        >>> import matplotlib.pyplot as plt
        >>> import seaborn as sns
        >>> tips = sns.load_dataset("tips")
        >>> sns.set_style("whitegrid")
        >>> g = sns.lmplot(x="tip",y="total_bill",data=tips,aspect=2)
        >>> g = (g.set_axis_labels("Tip","Total bill(USD)").set(xlim=(0,10),ylim=(0,100)))
        >>> plt.title("title")>>> plt.show(g)Step 4Step 2Step 1Step 5
    ```
    The Python visualization library Seaborn is based on matplotlib and provides a high-level interface for drawing attractive statistical graphics

    >>> import matplotlib.pyplot as plt
    >>> import seaborn as sns

    The basic steps to creating plots with Seaborn are:
        1. Prepare some data    
        2. Control figure aesthetics
        3. Plot with Seaborn  
        4. Further customize your plot


### Data

    Also see Lists, NumPy & Pandas

### Figure Aesthetics

    ```py
    f, ax = plt.subplots(figsize=(5,6) # Create a figure and one subplot
    ```
    Seaborn styles:
    ```py
        >>> sns.set() # (Re)set the seaborn default
        >>> sns.set_style("whitegrid")  # Set the matplotlib parameters
        >>> sns.set_style("ticks",{"xtick.major.size":8,"ytick.major.size":8}) # Set the matplotlib parameters
        >>> sns.axes_style("whitegrid") # Return a dict of params or use withwith to temporarily set the style
    ```