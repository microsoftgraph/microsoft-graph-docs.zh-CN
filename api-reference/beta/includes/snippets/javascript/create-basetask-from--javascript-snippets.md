---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02fbd58af59900173c1ac03ca7ee9d980e74f407
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525232"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tasks = {
  '@odata.type': '#microsoft.graph.baseTask',
  body: {
    '@odata.type': 'microsoft.graph.itemBody'
  },
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
  personalProperties: {
    '@odata.type': 'microsoft.graph.personalTaskProperties'
  }
};

await client.api('/me/tasks/lists/AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNi/tasks')
    .version('beta')
    .post(tasks);

```