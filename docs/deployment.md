# Deployment Guide

## Public Repository

If your repository is **public**, you can easily deploy your documentation using **GitHub Pages**. Here's how:

### 1. Navigate to Repository Settings

Go to your repository and click on the **Settings** tab.

![alt text](assets/images/settings-image.png)


### 2. Open the Pages Settings

Scroll down the left-hand sidebar and select **Pages**.

![alt text](assets/images/pages-image.png)

### 3. Configure the Source

Under the **Build and deployment** section:

* Set the **Source** to `Deploy from a branch`
* Select the `gh-pages` branch
* Click **Save**

![alt text](assets/images/branches-image.png)

After saving, GitHub will automatically trigger a **GitHub Action** that builds and deploys your documentation.

---

## Private Repository

If your repository is **private**, GitHub Pages might not be an option depending on your plan. In this case, you can run the documentation locally.

```bash
mkdocs serve
```

This will start a development server. Open your browser and visit:

```cpp
http://127.0.0.1:8000
```

You'll be able to preview and navigate through the documentation in real time.

---

## Further Examples

To see a real implementation example using this setup, check out the documentation inside the [FilterComp](https://github.com/Safe-Solutions-Engenharia/filtercomp) project.