---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68aa0860de0465c7f93975a4ff99b221efae083c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787416"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskFolder = {
  name: 'Volunteer'
};

await client.api('/me/outlook/taskfolders')
    .version('beta')
    .post(outlookTaskFolder);

```