---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29aa1261749e2b80a462b0fea667b61469471bb7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947749"
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