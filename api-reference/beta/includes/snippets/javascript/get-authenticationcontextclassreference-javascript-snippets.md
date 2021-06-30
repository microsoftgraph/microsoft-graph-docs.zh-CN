---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc0b9dc25af8c32b31d9997a3f717ff99fdbd94a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211917"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationContextClassReference = await client.api('/identity/conditionalAccess/authenticationContextClassReferences/c1')
    .version('beta')
    .get();

```