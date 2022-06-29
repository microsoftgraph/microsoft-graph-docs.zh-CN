---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8db609f42cb9d4e15ce85aca7f953a8f1e257d8
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66436243"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const checklistItem = {
    displayName: 'buy cake'
};

await client.api('/me/tasks/lists/AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA/checklistitems/e3a26c2e-7c6f-4317-9d71-c27267008202')
    .version('beta')
    .update(checklistItem);

```