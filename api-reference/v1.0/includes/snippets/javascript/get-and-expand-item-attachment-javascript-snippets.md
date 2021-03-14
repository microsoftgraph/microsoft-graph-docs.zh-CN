---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94a60a5c0b640787d39f094bce7bf6f4bed0739b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779455"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachment = await client.api('/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/')
    .expand('itemattachment/item')
    .get();

```