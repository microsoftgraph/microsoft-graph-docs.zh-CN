---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b91d035be91d30031f471226ce47acc684cf33d6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800131"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/external/connections/contosohr/groups/31bea3d537902000/members/14m1b9c38qe647f6a')
    .version('beta')
    .delete();

```