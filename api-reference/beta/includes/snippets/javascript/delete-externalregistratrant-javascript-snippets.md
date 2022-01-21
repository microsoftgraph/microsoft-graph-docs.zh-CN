---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7ef999fe0f6e505d4afbab71280404c2b532480
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103020"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants/9d96988d-a66a-46ce-aad7-0b245615b297')
    .version('beta')
    .delete();

```