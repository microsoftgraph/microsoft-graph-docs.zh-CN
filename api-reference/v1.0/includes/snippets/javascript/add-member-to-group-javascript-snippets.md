---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf2881189bc5dba3d36f5b31e567b6b504eec9b5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794319"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/directoryObjects/{id}'
};

await client.api('/groups/{group-id}/members/$ref')
    .post(directoryObject);

```