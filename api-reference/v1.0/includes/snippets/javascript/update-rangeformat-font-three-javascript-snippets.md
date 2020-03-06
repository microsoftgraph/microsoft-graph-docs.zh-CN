---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e5d5318e6b6e746eb123df30d8a2026a57d595b
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636780"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  underline: "Single",
  color: "#FFFFFF",
  size: 26
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/font')
    .update(workbookRangeFont);

```