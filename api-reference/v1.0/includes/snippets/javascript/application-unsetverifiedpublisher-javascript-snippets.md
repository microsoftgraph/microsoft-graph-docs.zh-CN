---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7abd5b19317a9e7a819937ad39b77703aa2eeaa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789781"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/unsetVerifiedPublisher')
    .post();

```