---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a62208cdb93a85bf916345056447fb630c9f4fab
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567032"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}')
    .get();

```