---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ee61f1624188cd4a1aae4a5a388dbe10e8a6dd4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808762"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationSynchronizationProfileStatus = await client.api('/education/synchronizationProfiles/{id}/profileStatus')
    .version('beta')
    .get();

```