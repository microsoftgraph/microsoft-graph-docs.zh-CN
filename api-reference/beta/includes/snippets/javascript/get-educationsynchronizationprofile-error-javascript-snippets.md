---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac59c7ef8a4abd8c7ce0e45de5fb7bc7d3175d08
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808289"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let errors = await client.api('/education/synchronizationProfiles/{id}/errors')
    .version('beta')
    .get();

```