# PA_MD_regression
Some clarification for things you'll see in the .rmd if you're not familiar with R.

The .rmd file with the code in it is an Rmarkdown file created using Rstudio.
The data used to generate the code was from SLF PA & MD operations.

Any code that looks like the following produces output when using Rmarkdown:

    ```{r,...}
    print(example %>% filter(example_variable <= 32 & example_variable >=5)

    ```

In the .rmd file you'll see a lot of the following:




    ```{r, echo=FALSE}
    
    
    ```
This means that I did not want the code to actually show up in the final product.
Many arguments can be used inside of the {r, ...} chunk for multiple different reasons, like handling errors and so on.

If there is a # inside of:

    ```{r, ...}
     
    # some text

    ggplot(example_ds, aes(x, y, fill) +
    geom_point() + ...

    ```
it's a comment.

If there's a # outside of the r code chunk it means the following string is a header.
One # is the largest header, and the more you use the smaller it gets. This is how you can organize which headers become clickable 
tabs in the ui for the final output.

If there's an asterisk (*) wrapping the text then that means some sort of effect is being added to the text itself.

1. One * for italics.
2. Two ** for bold.
3. Three *** for italics and bold.

Making an Rmarkdown file uses a lot of the same rules as making a README.md does here on github, so if you're familiar with 
that then the .rmd should be more recognizable.

