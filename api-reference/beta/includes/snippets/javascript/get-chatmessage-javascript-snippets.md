---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4d84c963bc4ecae3b3619e5ff5398cc37ce0f2d4
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/{id}/messages/{id}')
    .version('beta')
    .get();

```