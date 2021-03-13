---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: baee50503797381dfdb19dfd2831aeea981d3c88
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771734"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/shares/{printerShareId}/allowedUsers/{userId}/$ref')
    .delete();

```