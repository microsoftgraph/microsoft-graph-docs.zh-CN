---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34878fc56c5d97ca82e211862eeecd03439cfb7a93194d8f89a7e92cd94ed148
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104252"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let pivotTables = await client.api('/me/drive/root/workbook/worksheets/{id}/pivotTables')
    .get();

```