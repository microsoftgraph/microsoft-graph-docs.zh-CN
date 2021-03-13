---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba9e938de7c84d1150acef76839a8a49e1550300
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808754"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11021/assignments/19002/submissions/850f51b7/submit')
    .version('beta')
    .post();

```