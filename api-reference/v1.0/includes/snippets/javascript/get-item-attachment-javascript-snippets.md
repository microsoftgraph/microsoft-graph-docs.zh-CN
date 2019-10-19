---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68dff9a295a7b9c061ea93ab098a05fa3753057f
ms.sourcegitcommit: 6deec57c0ab736260ee3599703bfd3f567ee6d82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2019
ms.locfileid: "35739187"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=')
    .get();

```