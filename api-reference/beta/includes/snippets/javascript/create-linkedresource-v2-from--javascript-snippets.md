---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d846751915aeaf2b73c29672fec1ad69be919bb
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524763"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const linkedResources = {
    webUrl: 'https://microsoft.com',
    applicationName: 'Microsoft',
    displayName: 'Microsoft',
    externalId: 'dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9'
};

await client.api('/me/tasks/lists/AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA/linkedResources')
    .version('beta')
    .post(linkedResources);

```