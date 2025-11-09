# Assignment

## Brief

Write the Python codes for the following questions.

## Instructions

Paste the answer as Python in the answer code section below each question.

### Question 1

Question: How do you create a 2x2 subplot grid in matplotlib and select the first subplot?

Answer:

```
# Create the first subplot in a 2x2 grid
plt.subplot(2, 2, 1)  # (rows, cols, index)
plt.plot([1, 2, 3], [4, 5, 6])
plt.title('First Subplot')

plt.tight_layout()
plt.show()

```

### Question 2

Question: How to plot a line and set the color to red and style to dash in a matplotlib plot?

```python
x = [1, 2, 3, 4]
y = [1, 4, 9, 16]
```

Answer:

```
plt.plot(x,y,color="red",linestyle ="--")
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Red Dashed Line Example')
plt.show()

```

### Question 3

Question: How to plot a histogram with 30 bins for `data` in matplotlib?

```python
data = np.random.randn(1000)
```

Answer:

```
data = np.random.randn(1000)

fig = plt.figure()
ax = fig.add_subplot()
#ax.plot(data)
ax.hist(data, bins=30, color="black", alpha=0.3)

```

### Question 4

Question: How can you set the x-axis and y-axis labels in a matplotlib plot?

Answer:

```
fig, ax = plt.subplots()
# set the random seed to ensure reproducibility
rng = np.random.default_rng(seed=111)
ax.plot(rng.standard_normal(1000).cumsum())

ax.set_xlabel("X Label")
ax.set_ylabel("Y Label")
ax.set_title("matplotlib plot")

```

### Question 5

Question: How do you create a bar plot in seaborn using the `tips` dataset to show the average tip amount per day?

```python
import seaborn as sns
tips = sns.load_dataset('tips')
```

Answer:

```
ssns.barplot(x="day", y="tip", data=tips)

# Add title and axis labels
plt.title('Average Tips Amt per day')
plt.xlabel('Day of the Week')
plt.ylabel('Average Tip')

# Show the plot
plt.show()

```

### Question 6

Question: How to create a box plot for total_bill categorized by day in the `tips` dataset using seaborn?

Answer:

```
sns.boxplot(x='day', y='total_bill', data=tips)

# Add title and axis labels
plt.title('Distribution of Total Bill by Day')
plt.xlabel('Day of the Week')
plt.ylabel('Total Bill ($)')

# Show the plot
plt.show()

```

## Submission

- Submit the URL of the GitHub Repository that contains your work to NTU black board.
- Should you reference the work of your classmate(s) or online resources, give them credit by adding either the name of your classmate or URL.
