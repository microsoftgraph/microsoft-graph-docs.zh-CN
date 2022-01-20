---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c4961fce9c6ffb4fa93afb3a853b01eb2b75fc8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089918"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const linkedResource_v2 = {
    webUrl: 'https://microsoft.com',
    applicationName: 'Microsoft',
    displayName: 'Microsoft Web page',
    externalId: 'dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9'
};

await client.api('/me/tasks/lists/AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA/linkedResources/e2c5ed75-7aa4-4f8e-84ab-98b5e0b56ee8')
    .version('beta')
    .update(linkedResource_v2);

```