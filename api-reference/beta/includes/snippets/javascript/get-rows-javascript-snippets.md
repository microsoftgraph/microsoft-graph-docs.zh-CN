---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a4db2f59f25324c51c91d4fb0560cb9f7937016
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784209"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rows = await client.api('/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/rows')
    .version('beta')
    .get();

```