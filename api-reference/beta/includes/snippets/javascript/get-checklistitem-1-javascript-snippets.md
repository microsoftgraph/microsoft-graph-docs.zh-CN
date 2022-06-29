---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31fb52aed56bd89ace1a9d38bcc695b5f6f82337
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66440768"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let checklistItem = await client.api('/me/todo/lists/AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA/checklistitems/51d8a471-2e9d-4f53-9937-c33a8742d28f')
    .version('beta')
    .get();

```