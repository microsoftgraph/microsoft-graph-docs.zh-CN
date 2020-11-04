---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f99a6a2691bb9f01932135c4fd904ba2d6fcc9bf
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905369"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/headerRowRange')
    .get();

```