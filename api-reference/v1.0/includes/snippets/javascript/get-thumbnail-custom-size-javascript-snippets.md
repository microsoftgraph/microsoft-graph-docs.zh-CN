---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35ce3435e25254bb326a719eca9b52f6619c47f8
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let thumbnails = await client.api('/me/drive/items/{item-id}/thumbnails?select=c300x400_crop')
    .get();

```