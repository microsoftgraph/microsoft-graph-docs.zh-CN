---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 891368ace32cd6e6a57d050861e9ce5b28b88e24
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470368"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignmentResource = {
  distributeForStudentWork: 'false'
};

await client.api('/education/classes/11021/assignments/19002/resources/850f51b7-1df9-4ec0-bd62-64a0214b9cbf')
    .version('beta')
    .update(educationAssignmentResource);

```