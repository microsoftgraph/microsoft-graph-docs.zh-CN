---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0be9a5dbfb1a33a3561e1c615f3e7409f21a916
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612585"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/')
    .expand('itemattachment/item')
    .get();

```