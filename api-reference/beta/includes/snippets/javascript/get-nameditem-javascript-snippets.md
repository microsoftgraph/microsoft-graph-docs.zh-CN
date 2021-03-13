---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f02ac7dbe171fc5d841c9a530f43b396a4836474
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792855"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookNamedItem = await client.api('/me/drive/items/{id}/workbook/names/{name}')
    .version('beta')
    .get();

```