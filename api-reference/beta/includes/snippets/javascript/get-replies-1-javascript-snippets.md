---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a8556b6309bb576114f2684afbbe8773caa0ae9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let replies = await client.api('/chats/{id}/messages/{id}/replies')
    .version('beta')
    .get();

```