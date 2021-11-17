---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cff383bf45fbb3ccc67aff60720690e81cae3e66cee24013d5a092d2352d0c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902912"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachment = await client.api('/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/')
    .version('beta')
    .expand('itemattachment/item')
    .get();

```