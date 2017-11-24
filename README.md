# STEPS TO DEPLOY NODE APP WITH AWS EC2 Redhat/Amazon Linux Container Instance
<hr/>
<img width="100" height="100" src="https://pbs.twimg.com/profile_images/476766169349636096/xUHXk6zu.png" />
<img width="200" height="150" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAR8AAACvCAMAAADzNCq+AAAA/FBMVEX///8zMzNon2M+hj0uLi5rv0dZWVlyqWJ1rGQrKytxqGF2rmN3sGNtpV94sWJhm1xbmFV5tGF3tl0jIyN3d3dmn1tkZGR1t1lyuVWpqamwy65jmlhVlE5wu1Hx9fG+07zs8+xOkEk5OTkaGhoXFxcODg5Wmkx/f39ISEgxgTAAAAB+rHpYoklWmE3JycmcnJzl5eXc59u7u7ve3t6HsYOavZe1zrNPT0+vr6/N3sxYpUh2p3KiwqAlfCPJ28iSkpKGuH6Er4BpaWmHvXyZwI6bx4x7e3tAijlop1Kwz6fExMSCxmme0YxfuzS63a/Q58hVqUB3vFlKlkJClzS+M1XHAAANUUlEQVR4nO2de0ObyBrGSaC2aTcLbhpbEQmRGC9pNJiL1cS4uru16+5pPZ7v/10OtwHmyguJJgrPH7tVYSA/3nnm9g6RpJet4eH5yarvYZ31raZ0Noarvov11cdapaLsfxys+j7WVR6fSqXWuV71jaypAj6VSqOxvepbWUshPi6hvftV38waKuZTKY2aoQSf0qgZwviURk2J4OMZ9dmq72mdRPGpVI7LDnUsBp/ax1Xf1BqJwUfZWPVNrZFKPmKVfMQq+YhV8hGr5CNWyUesko9YJR+xSj5ilXzEKvmIVfIRq+QjVslHrJKPWCUfsUo+YpV8xCr5iFXyEavkI1bJR6ySj1glH7FKPmKtls9w+6v5bBfLpYX5LJAwNLjdbywrr8/880N9tpSSJOnk4CBK0ViQz7XdyZ2Wd73vX7uxt4R8kb+/f3j3TjNai5ckDTY6tVqUSrcQn6+NRu60vLNaA12vs7Vg1trPzU0Xz7u3O0bVWawkSTrYV/yb2j/wa/4CfE4O7fCEsKwMGp7biSvW9hfJWnP++O3XX1w+b982d3b6I2uBooInHt6UX/Nz8xncdpQKXhZYg4/7Cn7NRuNrrs/jGs9fnzY3Qz5vd3Z2tH5+G4qeeHhTeydDig6Qz3UHB5vFRU5t+qFU7MNcNvTj86ffYj71HY+Qls+GBlsd4qkpDZu+UQif2Dzis6Auwjg3WwEJ/fzs4on5vH+/46ufx4bC5iJdqXyGhyysMBfBjSdHAQk5m7ufP+F86gGgZn+U0RETxrMgH9o8IqW6iMk/NyigBrch8983Hh6cz/tmCKjZ18ElUcazCJ/TjigM7UNRW880HrIAoA39ePNml+ZTDwPIBaQ150A6WFOzGJ+zSkoYKh1uCv6ZAglhpXMLsKGfHh0mHxRAXghNQTZENjX5+YjMI1Ktc5r73KCAVBty/vkPl08UQC6gZv/PVBviNRfZ+aSZR6SGQqXgm9+A5wYFCH3M/Nelw+cT1zBPKTYEf2qpfMTGg8smhhwA4yEK4NvQD59OOh8EqH7BpSNoagRi8rlPMx6ijOSQ434vawjzbejnboiHzwerYR6hHseGMj+18NZoPsONTA7vKRpyDDfsHA+JvZXI+gfREfFpEoCa/THDhlKbGp4oPuZBZjqegiHH8DgXHb+Ac+JG9JgOhA/C06w3+2QlG+QwnlAkn/uM7V9cUOdWkrZy46lUOrjPX9x1YXyaJJ96/QiPoEEe40EfC+czOM7/Ae1tKf/JbgDhPYVR29jNxCeqYfXm0QQr6iDnI/dE8Pmas5qGReU/meJz0zb6MD4koLp8hLfzi0Q1wWd7AT6VwyXzMR6y8QnjxygMHwPGh7Bo+WXyUWzbFpXO4nOZjY9fw4yMfGpCd8rCx/2EwrKEfNxOsjkQddJYfAwYH6yGyZn4uB2vb6IODZyPYm+cDKlZyaQEfNBcj2BoRvLpe3y+wPhoMaB2Fj7BNKZoXAbm06j4/ZMTwfCByyc5SOfeDMWn348DKI1PDEjOwCeaR+fPxgD5JOYxthu8OnIo7TEvQcw1cyYZCD69bt8j9AXIBwFqw/nU7MQ6zClnQhrER9n/mOiRmgecOsLmo1So0fk1K4SYfPphJxHKR5OhfJQOvo5nsucVIXzsc2Ie1R2FMg6r3TL5NBjDxVPGZQg+v3cDQF0YH0OLwwfCp0GvA58cMkIIwCeav7JGKprlPaOPU46HLD61AxqPJAH4PHZ9QkEApfPxAQXhA+Cj3LLu6pBxYCqf6IiZplY1NMt7SxbV8Ca5GHzYi62sAxl8PELdDHxkKB/2U9vIxWfL/0tLVauetDFrKT+cAFo+H5fQA4yPC8hYHZ+xVg2lGhSfaALxKfh0uzA+bQOFz0r4qIhPVTNxPko8Ab1MPl8iPpew+Gm7WkM+Ycdx+XwiQG04nzaw//NsfGp28mMtlw8iJD9m4OMRulsXPnjHcfl8fEJuQOxm4dNurwsfagF+mXwuv4SEXD53bzLxkVfKpx/yYby87Cn4+I77AOMjr4yPiRp4teqvntwfs15+t0Q+f4R8Hn0+d0A+8qrqlyQ5PZeQqqKlgQErGWCpfC4vo/CR5cssfJ41fioV9Md51WCtTT4dH1ePqM+3+xnER4bxqdQYLzbczjc+VeJsTEtI5wn4oPCR5S+w+IHyodsW9swfJH6UzgYwmXKZfB48PnIsYPzIQD7E+1XpfFY4H2+CFJYUvmw+jwk+j0A+sgHjg02KctPKoPPPsKTwZfORk/r8XxiftgHkE42NBPms8PULSFL4Uvk8PDxifB6BfNwAgq/v2OdDYT5rhvUvQE73cvng4SPLwPrlOlCG9UHFFmYsZVo/dW3oOfncyRQgEB85C58UZVxfxtZEnpgPGT6y/B3IR8bzW551/V1oQ3A+9C1TfCg8bgDB+Kw0P0FkQww+x8wc+wP6OgSfH/9j8PkO43OF7+m5XSA/qoYvdNx3IOd0eDZE8VGOmfnjkkS3GQQf8+iIAQjE50jFr3W2n5/PPjEOOQcluNQ4Od0kH2plMdY2mcpB8JHMmyuaTzedz9HVmLwWeDcTKYXO7j+AJWiybQjnw0itT35+4kq0UTkqTWgzjc/V1KKvJc474dJhbrYFbnBh2lCSDz4zzRI+5mEZeUsmK1lfzOdI4yTQ50hb536HCnCDFCOn+zDGR8xMc66UuGt2Qze7Igj9KuAj301YZQTKmEDP2XkTCLjBjtpagvgoAuPBFdsQZ4BnTfFK1ubzOaKMB1OWbTOpjxdoafYWi09ySSxVyIa4A2BHw0LoO4fPHct4cIF3PwAeL9CGjrGTfD7pxkNcKbAhwQTBBGvrmXzaPOPBBdqHAXy8ABuq7eMo9rzI/Jb5LSS+DQknUMYJG+rTfIy+wHhwpdpQhsebsknSbcKIMNxqdKDGg2u70TgWvtojaUO//ELw6aZMi2MS7/zL+K1Nou2ajG1t5nXe95eYp2mbmS/aKIT6ePz0040HF2fLevCZMj7ewS2Hdv6XROSWjmwoyaffBBkPLl6KKGtVI03MhNysHrwkjYNK1o74CLacWo4jqHWMipH7674o0691Mr/DZUkKbeh9yKfL3bLsTDVXAl8i22fYVnOOMNOnbfk55dtQ2+fT/Z235d0aaX6+QLzcyxDWPud8YwpSou+5YEmLS3fb+vq7t/U695UJuhZlU4TpAmxFwwTefEQGDc+DXlweC1uyzNHV0Yfvf/P+PA8zSVFCac/iF+UPE/jzWZl0X7Ht1dgyJUtvCYwnwDJ1JojQTGRDtr2A8eA6uV/zF/RFaTiq2qJ+4p2y7p9piQqNR9XQa7ecm5DQNEcv6bVpXg3rU/K1bResXxZRfv6WHypEq08FVRElshqQDb1uTaIYYbotii0N9hKl16bIY24s3iFMbyqGLGQ8oq5yYW3IHBsBHS1tCjG2IWxgcjGbvWJbCo2nKhqqR0r0rdGvzKluWfPF33S7nnLSjQfXPNrlF/5iajrzuSllnYJ8GXIMiPHgQjY09X+azKXReGJIZu+JbnGlCo0ny8sz/bkh/zT/rBtJGjmSYUqvkc+FBjUeXM7UDyHvn1Nv56jhtmjZS1l/TdyPqeYad3q7kfxtWiPTjx8f1KuT7n3KXGe2EJ+LmXQzl9qmI166f5nS0aeMZTlOoqm+0EdTr4WbjmYX2HERH2nk932c6pPf7ApE8zHbmmaEdm3O1GgaWlU1bWzFx8V8pNlUn4yyvkD6ZYjmY2moYZIcNd7xGDAy4g52K3mmc/Eq6Yj5oK5RoIBQ3BFo0TXzFUrEJ+jjqL2ZPtH1cS+oaQbypsLz8Zp+N16iP5q6Dwz1AgvPZ+pFDzagn/udSSv4ofB8/PDBAYy83mQ4k1HyqVJdR280ooZzYyWfahwsSL1eb1rGT8Bn5AfQTctin1l4PhfhVKqmTsf6nEqUKjwf6SbOcPEGF+pIT06hlnykUfRCsBCTllgbK/m4VcztNONjMDX6Sr6SjydzPutVNS2BSSvbrwSf8HdOSx9V0TJQ8LuSDymz5S8FhUuDReczGY/HFKZeNepAF52P36iTh8+9AVgwz1x0Pjee1ZBrxj6fMn48PjMPxYg43FvUCec8is7H0WKvQWppcVAVnY/U8xur6gSNvKy5nySkhhOIhedjovGp2zsM/1st5w+T6xfk8o5Pq5yfj/qH5lhTCTpx6mHJx/tBn/pjLzWY4Zgl2vsC8cF+Q40vnHlrout668LCjisGn5ZKNuL88Rcmq0cvb7xCBb2caiIb1dKobg9DM79xe40ZP4SCSVQt/kpPSPyEX8QAe9/Cy5aJ0ldRdpyeWANkK0rxLUaWOEr5DpLDk0MIpswRM0X8FSvaXKD1RkE0qfyDdSPcYpAt4/VlC21OCf/Ht5/CblGZJHrKKq9ZKvIWJ3OmqWHNISd90BFF3yLX8pYopjNObKBNBUYxWq2MKrfoYnLwPZbcfbvFlDPSklvlCm88uKxgpjDa8YReMVEaT6hwb07gNZHxiF5RUjS1UFM/Q4OJLNvnCqDIcpJDs1IJoSYrObQvlVSwD1dNTA2VwqVPq9XRmhnP/wE5mEtmitz/3gAAAABJRU5ErkJggg==" />

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
