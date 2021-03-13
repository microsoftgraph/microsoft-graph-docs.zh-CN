---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba70ee5000806e8fd5e3e403ffb8a26cf2281c0c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799647"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let credentialUserRegistrationDetails = await client.api('/reports/credentialUserRegistrationDetails')
    .version('beta')
    .get();

```