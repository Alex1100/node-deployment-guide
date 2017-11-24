# STEPS TO DEPLOY NODE APP WITH AWS EC2 Redhat/Amazon Linux Container Instance
<hr/>
<img width="100" height="100" src="https://pbs.twimg.com/profile_images/476766169349636096/xUHXk6zu.png" />
<img width="200" height="150" src="http://yannickloriot.com/wp-content/uploads/2016/04/nodejs_logo_2016.png" />

<ol>
    <li>
        <p>Launch New EC2 Instance in AWS console</p>
    <li>
        <p>Define Security Groups</p>
        <p>Include public ip addr as custom tcp rule for security group</p>
    </li>
    <li>
        <p>Skip all steps and Launch</p>
    </li>
    <li>
        <p>Download New Pem file or use previous pem file</p>
    </li>
    <li>
        <p>chmod 400 Pem file</p>
    </li>
    <li>
        <p>ssh into machine by running <code>ssh -i ~/directory-of-pem-file/pemfile ec2user@public ip address of launched instance</code></p>
    </li>
    <li>
        <p>Prepare the Newly Launched Machine's System</p>
    </li>
    <li>
        <p>run <code>sudo yum install -y curl gpg gcc gcc-c++ make</code></p>
    </li>
    <li>
        <p>run <code>sudo gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3</code></p>
    </li>
    <li>
        <h3>For Red Hat, CentOS, Fedora, Amazon Linux, Scientific Linux</h3>
        <p>run <code>sudo yum install -y epel-release</code></p>
    </li>
    <li>
        <h3>For Node LTS version</h3>
        <p>run <code>curl --silent --location https://rpm.nodesource.com/setup_8.x | sudo bash -</code></p>
        <br/>
        <h3>For Node Unstable Latest</h3>
        <p>run <code>curl --silent --location https://rpm.nodesource.com/setup_9.x | sudo bash -</code></p>
    </li>
    <li>
        <p>run <code>sudo yum install gcc-c++ make</code></p>
    </li>
    <li>
        <p>run <code>sudo yum install -y --enablerepo=epel nodejs npm</code></p>
    </li>
    <li>
        <h3>To Install Yarn For CentOS, Fedora, AWS Linux, Redhat, Redhat Enterprise Linux</h3>
        <p>run 
            <code>
                sudo wget https://dl.yarnpkg.com/rpm/yarn.repo -O /etc/yum.repos.d/yarn.repo
            </code>
        </p>
    </li>
    <li>
        <p>run <code>sudo yum install yarn</code></p>
    </li>
    <li>
        <h3>Installing Git</h3>
        <p>run <code>sudo yum upgrade</code></p>
        <p>run <code>sudo yum instal git</code></p>
    </li>
    <li>
        <h3>Clone Git Repo to the SSH'ed Machine</h3>
        <p>run <code>git clone __cloned_repo_url__</code></p>
    </li>
    <li>
        <p>run <code>cd __name_of_cloned_repo__</code></p>
    </li>
    <li>
        <p>run <code>npm install || yarn install</code></p>
    </li>
    <li>
        <p>Add ENV VARS via VIM</p>
    </li>
    <li>
        <h3>To test server and code</h3>
        <p>run <code>webpack -w</code>, once webpack is finished compiling, run <code>ctrl + c</code></p>
        <p>run <code>node __your_servers_main_file__.js</code>
    </li>
    <li>
        <h3>To keep detached screen running forever while running the server</h3>
        <p>run <code>screen node __your_servers_main_file__.js</code></p>
        <p>run <code>ctrl + A + D</code> to keep screen running but detach yourself from it</p>
        <p>run <code>screen -r</code> to view all running screen instance</p>
    </li>
</ol>
