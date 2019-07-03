---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 268d52a604c904c8970f3fa9bcfafe7fc5bbf051
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500733"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/revokeSignInSessions')
    .version('beta')
    .post();

```