---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5354424ac03b82cab55aa50a470678317e929214
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946807"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const checklistItem = {
    displayName: 'Final sign-off from the team'
};

await client.api('/me/todo/lists/AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA/checklistitems/')
    .version('beta')
    .post(checklistItem);

```