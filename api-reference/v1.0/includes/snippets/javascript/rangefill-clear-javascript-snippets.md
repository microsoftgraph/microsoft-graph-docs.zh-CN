---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4549920f74120e01cfd7bf03bc98c6a3d73d118b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794671"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill/clear')
    .post();

```