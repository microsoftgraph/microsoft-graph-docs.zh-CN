---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 319ee69cbfb1c24403c4ccf701d58a8d51724d29
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804520"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/unmerge')
    .version('beta')
    .post();

```