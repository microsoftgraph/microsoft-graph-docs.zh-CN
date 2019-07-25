---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e6131bd1f22bc729d7ea91c06310b13acb63912c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728183"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/EntireRow')
    .version('beta')
    .get();

```