---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3855e6f6d0ce7a6b3e46a5228015bd4f02518109
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792098"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversation = await client.api('/groups/{id}/conversations/{id}')
    .get();

```