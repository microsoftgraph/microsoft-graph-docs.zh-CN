---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 517b4e89eb72020a46ac61666ad5a2873bd171aa
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472996"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationSubmission = await client.api('/education/classes/11010/assignments/19002/submissions/33223')
    .version('beta')
    .get();

```