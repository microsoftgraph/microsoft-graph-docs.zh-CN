---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 240f212c4358c84363e464aa8d76573400ec3213
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let signIn = await client.api('/auditLogs/signIns/{id}')
    .get();

```