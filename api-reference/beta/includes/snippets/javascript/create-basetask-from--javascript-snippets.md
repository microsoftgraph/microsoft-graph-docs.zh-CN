---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc5a1208ab9a9fe7f15defa5cfdd2be54df07be4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130104"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const baseTask = {
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
    .post(baseTask);

```