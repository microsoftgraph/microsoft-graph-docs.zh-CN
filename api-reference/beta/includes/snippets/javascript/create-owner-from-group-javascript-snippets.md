---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3dac2f0ca7834313ad70937223e31351c439d0f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799447"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/beta/users/{id}'
};

await client.api('/groups/{id}/owners/$ref')
    .version('beta')
    .post(directoryObject);

```