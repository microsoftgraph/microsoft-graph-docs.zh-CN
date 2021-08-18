---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c177afb15e1389f1ff0d19872eb3106962c20ffa112d5b7340eb48688e198fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163171"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let hostedContents = await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/replies/1616963389737/hostedContents')
    .version('beta')
    .get();

```