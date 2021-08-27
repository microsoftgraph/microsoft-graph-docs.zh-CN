---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3943495fe01fb37ba07a4722e6cbcedaea1cf2ccfced7cd37baa22824e5c5c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163167"
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