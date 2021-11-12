---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3771b77a186b77bb8b205f07b7ec065756b6b904b744b12ea323c1c1fff4a40f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218913"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTask = {
  dueDateTime: {
      dateTime: '2016-05-06T16:00:00',
      timeZone: 'Eastern Standard Time'
  }
};

await client.api('/me/outlook/tasks/AAMkADA1MTHgwAAA=')
    .version('beta')
    .update(outlookTask);

```