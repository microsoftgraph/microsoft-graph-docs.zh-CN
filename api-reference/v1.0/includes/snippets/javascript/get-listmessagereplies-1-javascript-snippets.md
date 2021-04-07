---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8334b701a99e1f1b202ec1e84bcb57cd6206c7ea
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611207"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let replies = await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616989510408/replies')
    .get();

```