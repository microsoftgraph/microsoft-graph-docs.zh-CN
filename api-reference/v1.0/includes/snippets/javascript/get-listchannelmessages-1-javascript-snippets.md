---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 499d6e948fd566e17a4895f9934ee409e6a2ee1cd0fb2971bb1559ff1958a7a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332120"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages')
    .get();

```