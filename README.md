# down_file_with_wget

### how to down file googledrive with wget??
#### Follow this instruction to do this 

Files can be downloaded from google drive using wget. Before that you need to know that files are small and large sized in google drive.

Files less than 100MB are regarded as small files where as files greater than 100MB are regarded as large files.

1. Select a file that is need to be downloaded and do right click.
2. Click Share. A dialog box will appear.
3. Click Advance in the right bottom corner.
4. Click on the Change.. under who has access.
5. Make it On- Public on the web.
6. Click Save button.
7. Copy the link for sharing…like…https://drive.google.com/file/d/1UibyVC_C2hoT_XEw15gPEwPW4yFyJFeOEA/view?usp=sharing
8. Extrac FILEID part like….from above….<strong>1UibyVC_C2hoT_XEw15gPEwPW4yFyJFeOEA</strong>


SO for small file run following command on your terminal:

`wget --no-check-certificate 'https://docs.google.com/uc?export=download&id=FILEID' -O FILENAME`
