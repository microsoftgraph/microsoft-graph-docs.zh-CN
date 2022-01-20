---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c56dfa8af7f04458feb68359aa32f451c6e82af
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106965"
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

await client.api('/me/tasks/lists/AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT')
    .version('beta')
    .update(baseTask);

```