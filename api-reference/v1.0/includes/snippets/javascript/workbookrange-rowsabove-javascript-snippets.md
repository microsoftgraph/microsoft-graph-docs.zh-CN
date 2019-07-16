---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cfe94f2615ebdd42bd23d60ce0a384efe9cda8c6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740518"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)')
    .post();

```