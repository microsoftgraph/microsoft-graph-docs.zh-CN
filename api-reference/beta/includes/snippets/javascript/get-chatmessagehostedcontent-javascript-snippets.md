---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a4e8fc4016ba86200e3df457522733f478947a55
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402159"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/{id}/messages/{id}/hostedContents/{id}/$value')
    .version('beta')
    .get();

```