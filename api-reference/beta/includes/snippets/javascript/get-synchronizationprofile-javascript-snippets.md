---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b52f20ed28bb53986c0edc3132c939097abeb8e5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780719"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/synchronizationProfiles/{id}')
    .version('beta')
    .delete();

```