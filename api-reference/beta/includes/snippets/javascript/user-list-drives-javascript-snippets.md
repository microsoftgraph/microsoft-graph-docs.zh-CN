---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b48780ca32c9a4b0aa47f6cf9643ed4e7dc1261
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783869"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/users/{userId}/drives')
    .version('beta')
    .get();

```