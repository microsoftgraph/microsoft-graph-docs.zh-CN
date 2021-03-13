---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29aa1261749e2b80a462b0fea667b61469471bb7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794666"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/chats/{id}/messages/{id}/hostedContents/{id}/$value')
    .version('beta')
    .get();

```