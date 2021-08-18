---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99d089acdb0745ea905e2f0e69731d0569cfd66508f05895b93e79995bfb40bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163170"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let hostedContents = await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents')
    .version('beta')
    .get();

```