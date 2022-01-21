---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2a4d336d594539dd8f02195bc93802172b024fe
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121517"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookTableRow = await client.api('/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/tableRowOperationResult(key='0195cfac-bd22-4f91-b276-dece0aa2378b')')
    .version('beta')
    .get();

```