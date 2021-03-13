---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f5f51cc9d09b16611a8b0733711d19f5db21cef
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792788"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/threads/{id}')
    .version('beta')
    .delete();

```