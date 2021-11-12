---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95df722f6db89d2ffdbbfba0adf276d79766c2aa8568422507b6e336359fa958
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignmentDefaults = {
  addedStudentAction: 'assignIfOpen',
  addToCalendarAction: 'studentsAndTeamOwners',
  notificationChannelUrl: 'https://graph.microsoft.com/beta/teams(\'id\')/channels(\'id\')'
};

await client.api('/education/classes/{id}/assignmentDefaults')
    .version('beta')
    .update(educationAssignmentDefaults);

```