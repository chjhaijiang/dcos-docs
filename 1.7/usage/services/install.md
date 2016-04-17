---
post_title: Installing Services
---
You can install services directly from the DC/OS package [repository][1], both via the web UI and the CLI.

**Prerequisite:**

*   [DC/OS][2] installed
*   [DC/OS CLI][3] installed

## Install a service with the CLI

1.  Install the datacenter service with this command:

         dcos package install <servicename>

    For example, to install Chronos:

         dcos package install chronos

## Install a service with the web UI

1.  Navigate to the Universe page in the DC/OS UI:

![Universe](/docs/1.7/usage/services/img/webui-universe-install.png)

2.  Click the green Install button next to the package you would like to install. You will see a dialog with another green Install button, and an option to proceed to an Advanced Installation. If you are an advanced user with a custom configuration to enter for this service, select the Advanced Installation; otherwise, click on Install Package.

## Verify your installation

*  From the DC/OS CLI: `dcos package list`
*  From the Mesosphere DC/OS web interface: Go to the Services tab and confirm that the datacenter services are running.
   ![services]()

    <a href="/wp-content/uploads/2015/12/services.png" rel="attachment wp-att-1126"><img src="/wp-content/uploads/2015/12/services-800x486.png" alt="Services page" width="800" height="486" class="alignnone size-large wp-image-1126" /></a>

 [1]: /docs/1.7/usage/package-repo/
 [2]: /docs/1.7/administration/installing/
 [3]: /docs/1.7/usage/cli/install/