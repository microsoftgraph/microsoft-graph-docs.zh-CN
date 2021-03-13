---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9b631940036d11628b7110c8084fc667b43166f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800867"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignmentDefaults = {
  addedStudentAction: 'assignIfOpen',
  notificationChannelUrl: 'https://graph.microsoft.com/beta/teams(\'id\')/channels(\'id\')'
};

await client.api('/education/classes/{id}/assignmentDefaults')
    .version('beta')
    .update(educationAssignmentDefaults);

```