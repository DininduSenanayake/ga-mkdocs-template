# `mkdocs-material` template for GA/NeSI workshops

* Template is based on `mkdocs-material`https://squidfunk.github.io/mkdocs-material/



!!! python "Install `mkdocs-material` and supplementary plugins locally"

    ```python
    pip install mkdocs-material 
    pip install mkdocs-glightbox
    pip install mkdocs-awesome-pages-plugin
    ```

!!! terminal-2 "1. Clone your repo and bootstrap it with `mkdocs-material`"
    * Replace `your-repo` wth the correct URL
    ```bash
    git clone https://github.com/your-repo/your-repo.git
    ```
    ```bash
    cd your-repo && mkdocs new .
    ```

!!! terminal-2 "2. Clone ths repo and replace the default config/stylesheets"

    ```bash
    git clone https://github.com/DininduSenanayake/ga-mkdocs-template.git
    ```

    * copy/replace the following files/folders in `your-repo` with the ones from `ga=mkdocs-template`
    ```bash
    ga-mkdocs-template/mkdocs.yml
    ga-mkdocs-template/.github
    ga-mkdocs-docs/docs/javascripts
    ga-mkdocs-template/docs/stylesheets
    ```

!!! terminal-2 "3. Replace `mkdocs.yml` line 1-9 with information related to your repo" 

    ```bash linenums="1"
    site_name: GA/NeSI mkdocs-material theme
    site_author: Genomics Aotearoa & NeSI
    site_dir: public
    site_url: "https://dinindusenanayakeithub.io/ga-mkdocs-template/"

    #Repository information

    repo_name:  DininduSenanayake/ga-mkdocs-template
    repo_url: https://github.com/DininduSenanayake/ga-mkdocs-template

    
    ```


!!! terminal-2 "4. Deploy - Only has to do this once"

    ```bash
    mkdocs gh-deploy
    ```

    * This manual deployment is only for the first round. All subsequent builds will be done by github actions as per `.github/workflows/ci.yml`
