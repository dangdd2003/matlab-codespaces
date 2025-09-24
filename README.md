# Run MATLAB in GitHub Codespaces

This repository shows how to run MATLAB&reg; in [GitHub&trade; Codespaces](https://github.com/features/codespaces), so you can quickly start a development environment for developing the MATLAB code hosted in your Github repository.


## Table of Contents
- [When Should I Use MATLAB in Codespaces?](#when-should-i-use-matlab-in-codespaces)
- [Choose a Configuration](#choose-a-configuration)
- [Use MATLAB in Codespaces](#use-matlab-in-codespaces)
  - [What Can I Do With MATLAB in VS Code?](#what-can-i-do-with-matlab-in-vs-code)
  - [What Can I Do With MATLAB in JupyterLab?](#what-can-i-do-with-matlab-in-jupyterlab)
- [Related Links](#related-links)    


## When Should I Use MATLAB in Codespaces?

A [codespace (GitHub Docs)](https://docs.github.com/en/codespaces/overview) is a development environment you run in the cloud. If you own a Github repository hosting MATLAB code, users of your repository can use Codespaces to:
- Configure a consistent and customizable development environment.
- Run MATLAB along with other software or programming languages.
- Use Git to contribute back to your repository.

## Choose a Configuration

Codespaces run in Docker containers called development containers, or [dev containers (GitHub Docs)](https://docs.github.com/en/codespaces/setting-up-your-project-for-codespaces/adding-a-dev-container-configuration/introduction-to-dev-containers). You can customize how MATLAB is installed in your codespace by modifying the configuration file of the dev container, named `devcontainer.json`. Choose the configuration that corresponds to your desired use case.

| Use Case  | Recommendation | Start Codespace Using Recommended Configuration |
| ------------- | ------------- |------------- |
|Use MATLAB only|Use a prebuilt [MATLAB Container on Docker Hub](https://hub.docker.com/r/mathworks/matlab). <br><br>Configure your codespace using this [devcontainer.json](.devcontainer/devcontainer.json).|[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new/mathworks-ref-arch/matlab-codespaces?template=false&devcontainer_path=.devcontainer%2Fdevcontainer.json)|
|Customize MATLAB installation with specific toolboxes or other software|Create a custom MATLAB container image using [MATLAB Dockerfile](https://github.com/mathworks-ref-arch/matlab-dockerfile). You can see an example Dockerfile in the `.devcontainer/using-matlab-dockerfile` folder. <br><br>Configure your codespace using this [devcontainer.json](.devcontainer/using-matlab-dockerfile/devcontainer.json).|[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new/mathworks-ref-arch/matlab-codespaces?template=false&devcontainer_path=.devcontainer%2Fusing-matlab-dockerfile%2Fdevcontainer.json)|
|Add MATLAB to an existing devcontainer configuration|Use the [MATLAB Feature for Devcontainers](https://github.com/mathworks/devcontainer-features/tree/main/src/matlab). <br><br>Configure your codespace using this [devcontainer.json](.devcontainer/using-devcontainer-feature/devcontainer.json).|[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new/mathworks-ref-arch/matlab-codespaces?template=false&devcontainer_path=.devcontainer%2Fusing-devcontainer-feature%2Fdevcontainer.json)||

## Use MATLAB in Codespaces 

Use your MATLAB codespace to:
- Run & Debug `.m` files in VS Code
- Run MATLAB code in Jupyter Notebooks in both VS Code and JupyterLab
- Switch to the MATLAB IDE to use more MATLAB features.

By default, your MATLAB codespace starts in a [Visual Studio Code](https://code.visualstudio.com/) environment, and MATLAB opens in a browser tab.

![VSCode In Codespaces](img/VSCodeInCodespaces.png)

For details on using MATLAB in VS Code in your codespace, see [What Can I Do With MATLAB in VS Code?](#what-can-i-do-with-matlab-in-vs-code)

For details on using MATLAB in JupyterLab in your codespace, see [What Can I Do With MATLAB in JupyterLab?](#what-can-i-do-with-matlab-in-jupyterlab)




### What Can I Do With MATLAB in VS Code?

Once you have MATLAB set up in your codespace, you can use VS Code to: 

1. **Run & Debug MATLAB files in the VS Code editor.**</br>
   
   ![Run and Debug MATLAB in VS Code](img/RunAndDebugInVSCode.gif)
   
   For more information, see [MATLAB Extension for Visual Studio Code](https://github.com/mathworks/MATLAB-extension-for-vscode).


2. **Access MATLAB in a browser tab.**</br>

   ![MATLAB Proxy](img/MATLABinBrowser.png)

   For more information on using MATLAB in the browser, see [MATLAB Proxy](https://github.com/mathworks/matlab-proxy).

3. **Run MATLAB code in Jupyter Notebooks within VS Code.**</br>

   You can run MATLAB code in Jupyter Notebooks, within the VS Code environment. For more information about VS Code support for Jupyter Notebooks, see [Jupyter Notebooks in VS Code (VS Code)](https://code.visualstudio.com/docs/datascience/jupyter-notebooks).
   
   ![Jupyter Notebook In VS Code](img/JupyterNotebookInVSCode.gif)


### What Can I Do With MATLAB in JupyterLab?

The configurations in [Choose a Configuration](#choose-a-configuration) enable you to run MATLAB in JupyterLab as well as VS Code:

![Open In JupyterLab](img/OpenInJupyterLab.gif)


After opening JupyterLab in your codespace, you can:

1. **Run MATLAB code in Jupyter Notebooks.**</br>
   
   ![Run MATLAB code using Jupyter Notebooks](https://github.com/mathworks/jupyter-matlab-proxy/raw/main/img/JupyterKernel.gif)

2. **Access MATLAB in a browser window.**</br>
      
   ![Access the MATLAB in a browser window](https://github.com/mathworks/jupyter-matlab-proxy/raw/main/img/JupyterMATLABDesktop.gif)


## Related Links 
- [Overview of Codespaces (GitHub)](https://docs.github.com/en/codespaces/overview)
- [Development Container Features (GitHub)](https://github.com/devcontainers/features/)
- [Development Container Specification (Microsoft&reg;)](https://containers.dev/implementors/spec/)
- [Setting Your Default Editor for Codespaces (GitHub)](https://docs.github.com/en/codespaces/setting-your-user-preferences/setting-your-default-editor-for-github-codespaces)
- [Run Dev Containers in VS Code (VS Code Docs) ](https://code.visualstudio.com/docs/devcontainers/create-dev-container)

---

Copyright 2024-2025 The MathWorks, Inc.

---
