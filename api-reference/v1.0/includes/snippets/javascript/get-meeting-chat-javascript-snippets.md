---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4666eadcd48001fb881ce7c4ecee607489f6c01f
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519698"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chat = await client.api('/chats/19:meeting_ZDZlYTYxOWUtYzdlMi00ZmMxLWIxMTAtN2YzODZlZjAxYzI4@thread.v2')
    .get();

```