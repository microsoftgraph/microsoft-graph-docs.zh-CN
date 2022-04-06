---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f637d0b372192756c1c60b3323df89c56209ccfb
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528081"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const baseTask = {
  '@odata.type': '#microsoft.graph.task',
  textBody: 'String',
  bodyLastModifiedDateTime: 'String (timestamp)',
  completedDateTime: 'String (timestamp)',
  dueDateTime: {
    '@odata.type': 'microsoft.graph.dateTimeTimeZone'
  },
  startDateTime: {
    '@odata.type': 'microsoft.graph.dateTimeTimeZone'
  },
  importance: 'String',
  recurrence: {
    '@odata.type': 'microsoft.graph.patternedRecurrence'
  },
  displayName: 'String',
  status: 'String',
  viewpoint: {
    '@odata.type': 'microsoft.graph.taskViewpoint'
  }
};

await client.api('/me/tasks/lists/AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNi/tasks')
    .version('beta')
    .post(baseTask);

```