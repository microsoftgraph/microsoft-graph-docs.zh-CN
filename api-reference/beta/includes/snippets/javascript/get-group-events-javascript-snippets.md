---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47c92a6cea3cb43b68489e698b06776477ca5cdd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788522"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let events = await client.api('/groups/{id}/events')
    .version('beta')
    .get();

```