---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97f99543cc7766c420b352f00c0421a25fe44dc9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778120"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/trustFramework/keySets/{id}')
    .version('beta')
    .delete();

```