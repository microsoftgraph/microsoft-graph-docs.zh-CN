---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0d1d5f692a1d90c467d91ef1460cb046cb28394f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480188"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/thumbnails?select=c300x400_Crop')
    .version('beta')
    .get();

```