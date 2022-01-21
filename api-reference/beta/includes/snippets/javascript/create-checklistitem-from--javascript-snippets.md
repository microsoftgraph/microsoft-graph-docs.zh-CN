---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6b86386780a8406bd075a49933ac91036b27a9f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114207"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const checklistItem = {
    displayName: 'Final sign-off from the team'
};

await client.api('/me/tasks/lists/AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA/checklistitems/')
    .version('beta')
    .post(checklistItem);

```