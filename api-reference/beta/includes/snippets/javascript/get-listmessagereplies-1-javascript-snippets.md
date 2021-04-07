---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae0668cb2c476072e50adf9497a92c670bb2d432
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610156"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let replies = await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616989510408/replies')
    .version('beta')
    .get();

```