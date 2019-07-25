---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 733dd832a0712ff3d7c9a48067cd65d283c2f961
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713022"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/checkout')
    .version('beta')
    .post();

```