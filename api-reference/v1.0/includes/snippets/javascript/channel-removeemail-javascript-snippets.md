---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 515b1c88dddeb633abaa9339f20bac1e64c23c2c
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777158"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/removeEmail')
    .version('beta')
    .post();

```