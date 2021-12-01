# GitHub repo template to promote reproducible clinical metabolomics study

### Checklist

- [ ] Deposit data to a public repository
- [ ] Present metadata clearly
- [ ] Share workflow components information with a version control system
- [ ] Use open-source and downloadable software
- [ ] Use virtual machine or software container
- [ ] Document runtime hardware information
- [ ] Semantic annotation for workflow components
- [ ] Use workflow automation or literate programming

### Computational resource information (with examples)

- **Public repository used to deposit data:** MetaboLights
- **Unique identifier of data deposited to a public repository:** MTBLS1
- **Template used to present metadata in the manuscript:** Cell STAR★Methods
- **Version control system used to share computational resource information:** GitHub
- **Used software names along with versions (if applicable) and URL used in the analysis:** ProteoWizard-msConvert (https://proteowizard.sourceforge.io/tools.shtml), MS-DIAL v4.46 (http://prime.psc.riken.jp/compms/msdial/main.html), 
- **URL of shared project file:** https://s3.console.aws.amazon.com/s3/buckets/example
- **URL of shared virtual machine or software container used for the analysis:** https://hub.docker.com/_/python
- **Model of runtime CPU: Intel Core i7
- **Number of runtime CPU: 6
- **Model runtime GPU: NVDIA GeForce GTX 980 Ti
- **Number of runtime GPU: 2
- **Ontology used for semantic annotation of the analysis workflow:** EDAM Ontology
- **Tool used for workflow automation or literate programming:** Nextflow v20.07.1 (https://www.nextflow.io/index.html)
- **Order of running workflow components:**
    1. Use ProteoWizard-msConvert to convert data from .RAW format to .mzML format, store the converted data to `data/` folder
    2. Run Nextflow pipeline by typing the following command:
    ```
    nextflow main.nf
    ```
