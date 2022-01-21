---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25538233be9fd642b034364bb52462eebfb2a032
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102964"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let registrants = await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants')
    .version('beta')
    .get();

```