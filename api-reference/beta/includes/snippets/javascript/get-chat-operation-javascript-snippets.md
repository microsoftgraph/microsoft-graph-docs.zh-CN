---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9217b35090161956b0d8bb1625dfd4c463b2073
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210264"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsAsyncOperation = await client.api('/chats/19:c253a29b5f694b55a6baad8e83510af7@thread.v2/operations/2432b57b-0abd-43db-aa7b-16eadd115d34-e88ae9aa-887e-4972-ac3e-bd578e38232e-cf58835e-43f0-4fc1-825e-5de55630e7e4')
    .version('beta')
    .get();

```