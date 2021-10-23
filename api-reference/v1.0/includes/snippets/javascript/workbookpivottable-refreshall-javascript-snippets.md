---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac0acc0a606f7104904ff600534d1960c9a30943
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60562770"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/root/workbook/worksheets/{id|name}/pivotTables/refreshAll')
    .post();

```