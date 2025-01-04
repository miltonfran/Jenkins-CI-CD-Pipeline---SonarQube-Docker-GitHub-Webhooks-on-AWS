<h1>Jenkins CI/CD Pipeline - SonarQube, Docker, GitHub Webhooks on AWS</h1>


<h2>Description</h2>
This project demonstrates the implementation of a Continuous Integration and Continuous Deployment (CI/CD) pipeline using Jenkins. The pipeline integrates tools like SonarQube for code quality analysis, Docker for containerization, and GitHub webhooks for automating build and deployment processes. The entire pipeline is deployed and managed on AWS, showcasing modern DevOps practices for automating software delivery in cloud environments.
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735937332/Screenshot_2025-01-03_121418_l7tcej.png"/>
<br />


<h2>Languages and Utilities Used</h2>
Programming Languages:

- <b>Java (used for the sample application being built)<b>

YAML (for Jenkins pipeline configuration)
- <b>Scripting:
Shell scripting for automating pipeline steps.<b>

<h2>Tools and Technologies:</h2>
CI/CD Tool:

Jenkins (pipeline automation)

Code Quality and Static Analysis:

SonarQube
Containerization:
Docker

Version Control:

GitHub (with webhooks integration)

Cloud Platform:

AWS (EC2 instances for Jenkins, SonarQube, and Docker)


<h2>Environments Used </h2>

Environment:
Operating System:

Ubuntu (used on EC2 instances)

AWS Resources:

EC2 (for hosting Jenkins, SonarQube, and the application)
S3 (optional, for storing artifacts)

Network Setup:

Private VPC (for security)
Security Groups (to allow specific inbound/outbound traffic)


<h2>Program walk-through:</h2>

<p align="center">
Step 1: Setting up the AWS Environment
Get free CSS
Launch an EC2 instance on AWS for Jenkins and configure security groups.
Install Java and Jenkins on the EC2 instance.
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735936816/Screenshot_2025-01-02_181204_nl7alj.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735936951/Screenshot_2025-01-02_183056_qzr1gd.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735937146/Screenshot_2025-01-02_184244_mn5jbl.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735937233/Screenshot_2025-01-02_185612_iaqmex.png"/>
<br />
<br />
Step 2: Installing and Configuring Jenkins
Access Jenkins through its web UI.
Install necessary plugins (e.g., GitHub Integration, Docker Pipeline, SonarQube Scanner).
  <br/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735940893/Screenshot_2025-01-02_192539_qexgpk.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735940664/Screenshot_2025-01-02_192434_yvdzrf.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735941075/Screenshot_2025-01-02_193103_vhmllt.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735941183/Screenshot_2025-01-02_193216_wglsfp.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735941267/Screenshot_2025-01-02_193514_c2npha.png"/>
<br />
<br />

Step 3: Setting up GitHub Repository
Create or clone a GitHub repository for the Java application.
Configure GitHub webhooks to trigger Jenkins builds on push events. <br/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735941498/Screenshot_2025-01-02_195307_xza8ba.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735941547/Screenshot_2025-01-02_195420_dktxan.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735941608/Screenshot_2025-01-02_195513_qjxqft.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735941672/Screenshot_2025-01-03_120546_b6a6as.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735941980/Screenshot_2025-01-03_120615_sljnse.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942019/Screenshot_2025-01-03_120655_mwuqkp.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942073/Screenshot_2025-01-03_120721_xxt58b.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942100/Screenshot_2025-01-03_120735_ey3lpo.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942236/Screenshot_2025-01-03_120751_vkwvjc.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942285/Screenshot_2025-01-03_120812_f74hhj.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942317/Screenshot_2025-01-03_120837_bftm7k.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942352/Screenshot_2025-01-03_120850_s6rusr.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942387/Screenshot_2025-01-03_120915_oqszko.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942482/Screenshot_2025-01-03_120940_syhym5.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942507/Screenshot_2025-01-03_121029_pojiri.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942534/Screenshot_2025-01-03_121044_n1ecdz.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942557/Screenshot_2025-01-03_121330_x6fdr4.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942584/Screenshot_2025-01-03_121351_bwv8ih.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942620/Screenshot_2025-01-03_121451_dcr5k1.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942653/Screenshot_2025-01-03_121517_dhvhh2.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942765/Screenshot_2025-01-03_121721_cpeiau.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942789/Screenshot_2025-01-03_121736_pxpcao.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942910/Screenshot_2025-01-03_121816_odar7a.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942934/Screenshot_2025-01-03_121907_mv8etp.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735942980/Screenshot_2025-01-03_121935_n6b8jd.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735943033/Screenshot_2025-01-03_122903_zo0epm.png"/>
<br />
<br />

Step 4: Installing and Configuring SonarQube
Launch another EC2 instance for SonarQube.
Install and configure SonarQube.
Generate SonarQube tokens and integrate them into Jenkins.
  <br/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735943816/Screenshot_2025-01-03_122935_ngydwd.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735943916/Screenshot_2025-01-03_122947_bq1umi.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735943937/Screenshot_2025-01-03_123008_ok6atg.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735943955/Screenshot_2025-01-03_123140_rfjgpo.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735943981/Screenshot_2025-01-03_123202_eiybw6.png
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944004/Screenshot_2025-01-03_123334_pylljk.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944025/Screenshot_2025-01-03_123444_lgnzty.png
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944134/Screenshot_2025-01-03_123502_ty24ax.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944158/Screenshot_2025-01-03_123917_bajouw.png
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944340/Screenshot_2025-01-03_123935_iqqjq3.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944360/Screenshot_2025-01-03_123949_x7r61d.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944567/Screenshot_2025-01-03_124215_rkzklq.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944588/Screenshot_2025-01-03_124246_bszxlk.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944621/Screenshot_2025-01-03_124301_a8d25z.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944639/Screenshot_2025-01-03_124317_e6brho.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944666/Screenshot_2025-01-03_125113_tie40t.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944690/Screenshot_2025-01-03_125142_rxg59d.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944714/Screenshot_2025-01-03_125204_mjw47u.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944735/Screenshot_2025-01-03_125222_stc2h3.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944927/Screenshot_2025-01-03_125236_wyibvm.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944948/Screenshot_2025-01-03_125311_hta2fk.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944971/Screenshot_2025-01-03_125320_youk5o.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735944994/Screenshot_2025-01-03_125342_ph1b6h.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735945021/Screenshot_2025-01-03_125349_jyud7v.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735945062/Screenshot_2025-01-03_125342_zsyepj.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735945084/Screenshot_2025-01-03_125402_bqmad3.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735945108/Screenshot_2025-01-03_125411_i60djy.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735945144/Screenshot_2025-01-03_125446_hsfxm8.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735945180/Screenshot_2025-01-03_125927_mef72d.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735945209/Screenshot_2025-01-03_130142_eqbf25.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735946120/Screenshot_2025-01-03_130203_v9uwaa.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735946199/Screenshot_2025-01-03_130252_mfnnxq.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735946255/Screenshot_2025-01-03_130237_mqmoyj.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735946308/Screenshot_2025-01-03_130306_itoz66.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735946334/Screenshot_2025-01-03_130331_gzv3ti.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735946391/Screenshot_2025-01-03_130342_mu5n4v.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735946434/Screenshot_2025-01-03_130414_guiy4x.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735946476/Screenshot_2025-01-03_130421_l72qyi.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735946607/Screenshot_2025-01-03_132126_zcc85t.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735946656/Screenshot_2025-01-03_132135_qxc4mz.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735946695/Screenshot_2025-01-03_132206_eb6zhr.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735947468/Screenshot_2025-01-03_132517_her5co.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735947512/Screenshot_2025-01-03_132540_qdoh6d.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735947546/Screenshot_2025-01-03_132550_mep5ss.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735947584/Screenshot_2025-01-03_132658_qslw2q.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735947639/Screenshot_2025-01-03_132740_idqd1b.png"/>
<br />
<br />

Step 5: Creating a Docker Image
Write a Dockerfile for the application.
Build and push the Docker image to Docker Hub using Jenkins.
<br/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735948051/Screenshot_2025-01-03_133043_jdncoi.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735948907/Screenshot_2025-01-03_134723_qtwckw.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735949020/Screenshot_2025-01-03_134829_duddpk.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735949135/Screenshot_2025-01-03_135653_zmn2xg.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735949179/Screenshot_2025-01-03_135732_tocuva.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735949299/Screenshot_2025-01-03_135816_jrjj5s.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735949396/Screenshot_2025-01-03_135923_nzv12n.png"/>
<br />
<br />

Step 6: Setting Up Jenkins Pipeline
Write a Jenkins pipeline script (Jenkinsfile) with the following stages:
Clone the code from GitHub.
Build the application using Maven.
Perform static code analysis with SonarQube.
Build a Docker image for the application.
Deploy the application (either to a Docker container or AWS).

Step 7: Triggering the CI/CD Pipeline
Push changes to the GitHub repository to trigger the pipeline.
Monitor the pipeline execution in Jenkins.

Step 8: Testing and Deployment
Test the deployed application in the Docker container.
Access logs and validate the entire setup.
<br/>

<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735949721/Screenshot_2025-01-03_140137_jsgopc.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735950565/Screenshot_2025-01-03_140355_nitpcn.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735950565/Screenshot_2025-01-03_140355_nitpcn.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735950826/Screenshot_2025-01-03_141257_r7c1md.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735951322/Screenshot_2025-01-03_141312_j7gf5y.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735951692/Screenshot_2025-01-03_142814_lysz73.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735951722/Screenshot_2025-01-03_142853_ybqolb.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735951755/Screenshot_2025-01-03_142948_ktsmn7.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735951839/Screenshot_2025-01-03_143253_skkfe6.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735951886/Screenshot_2025-01-03_143321_h80jhc.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735952192/Screenshot_2025-01-03_143348_uju3b6.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735952221/Screenshot_2025-01-03_144142_ekw1ik.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735952323/Screenshot_2025-01-03_144309_yyvkha.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735952611/Screenshot_2025-01-03_144416_qpgzvn.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735952611/Screenshot_2025-01-03_144416_qpgzvn.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735952679/Screenshot_2025-01-03_144707_wokrye.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735952795/Screenshot_2025-01-03_144847_dxfmyx.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735952835/Screenshot_2025-01-03_145702_ptk8fu.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735952869/Screenshot_2025-01-03_150418_p4ccav.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735952935/Screenshot_2025-01-03_150433_rzc6pz.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1735952955/Screenshot_2025-01-03_150447_reflmm.png"/>

<br />
<br />
