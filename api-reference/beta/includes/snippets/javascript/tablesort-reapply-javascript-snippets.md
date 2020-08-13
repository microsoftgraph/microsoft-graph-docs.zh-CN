---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f767bf9504d3d49351b87a3be8714999bd47a9e4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724540"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort/reapply')
    .version('beta')
    .post();

```