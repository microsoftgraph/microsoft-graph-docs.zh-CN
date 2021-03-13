---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ffc35165c19637d23c9d5cba81ac5fa287e7f72
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806242"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  '@odata.id': 'https://graph.microsoft.com/beta/groups/{id}'
};

await client.api('/print/shares/{id}/allowedGroups/$ref')
    .version('beta')
    .post(group);

```