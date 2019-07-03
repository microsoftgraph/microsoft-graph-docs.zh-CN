---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ca7d0ad78cc7c3d6253157c4f303d5a752e233c1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510019"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const merge = {
  across: true
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/merge')
    .post(merge);

```