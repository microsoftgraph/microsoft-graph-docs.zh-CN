---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 806a9ca831d88fa7bb45e9ee4c64748c56ae75af
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774143"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{userId}/profile/awards/{personAwardId}')
    .version('beta')
    .delete();

```