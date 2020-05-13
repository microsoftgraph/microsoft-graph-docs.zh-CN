---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 733dd832a0712ff3d7c9a48067cd65d283c2f961
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
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