---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb9161bc69c4edda301e2a82d5f1cce6e412a57a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793063"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/me/assignments/{id}/rubric/$ref')
    .version('beta')
    .delete();

```