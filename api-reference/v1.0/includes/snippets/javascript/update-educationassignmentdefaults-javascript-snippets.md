---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0ed59bd1bfdbaaa601ba747f3d8a6a3c798e1af09ac4f6975301c1c410880ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333977"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignmentDefaults = {
  addedStudentAction: 'assignIfOpen',
  notificationChannelUrl: 'https://graph.microsoft.com/beta/teams(\'acdefc6b-2dc6-4e71-b1e9-6d9810ab1793\')/channels(\'3da03fc4-8eac-4459-84fb-1422dc01f65e\')'
};

await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentDefaults')
    .update(educationAssignmentDefaults);

```