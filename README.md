  <title>How to Set Up a Scalable Virtual Machine in Azure</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 2em; }
        h1 { color: #0078d4; }
        code, pre { background: #f4f4f4; padding: 2px 6px; border-radius: 4px; }
        ol { margin-left: 1.5em; }
    </style>
</head>
<body>
    <h1>How to Set Up a Scalable Virtual Machine in Azure</h1>
    <p>
        This document provides detailed instructions on how to set up a scalable virtual machine in Azure.
    </p>
    <h2>Prerequisites</h2>
    <ul>
        <li>An active Azure account.</li>
        <li>Basic knowledge of Azure services and virtual machines.</li>
        <li>Azure CLI installed on your local machine.</li>
    </ul>
    
    <h2>Step-by-Step Setup Instructions</h2>
    <ol>
        <li>
            <strong>Log in to Azure:</strong>
            <pre>
az login
            </pre>
        </li>
        <li>
            <strong>Create a Resource Group:</strong>
            <pre>
az group create --name &lt;your-resource-group&gt; --location &lt;your-location&gt;
            </pre>
        </li>
        <li>
            <strong>Create a Virtual Machine:</strong>
            <pre>
az vm create --resource-group &lt;your-resource-group&gt; --name &lt;your-vm-name&gt; --image &lt;image-type&gt; --admin-username &lt;your-username&gt; --admin-password &lt;your-password&gt;
            </pre>
        </li>
        <li>
            <strong>Configure Scaling Options:</strong>
            <ul>
                <li>Set up auto-scaling based on metrics such as CPU usage or memory.</li>
                <li>Use Azure Scale Sets for managing multiple instances of your VM.</li>
            </ul>
        </li>
        <li>
            <strong>Networking Configuration:</strong>
            <ul>
                <li>Configure Virtual Network and Subnet settings.</li>
                <li>Set up Network Security Groups (NSGs) to control inbound and outbound traffic.</li>
            </ul>
        </li>
    </ol>

    <h2>Best Practices for Scaling</h2>
    <ul>
        <li>Monitor performance metrics regularly to adjust scaling settings.</li>
        <li>Use Azure Monitor and Azure Alerts to stay informed about your VM's performance.</li>
        <li>Consider using managed disks for better performance and scalability.</li>
    </ul>

    <p>
        For more details, refer to the <a href="https://learn.microsoft.com/en-us/azure/virtual-machines/">Azure Virtual Machines Documentation</a>.
    </p>
</body>
</html>
