---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5da9e49fce039017950593318e05bf9f928ac4f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804458"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let alert = await client.api('/security/alerts/{id}')
    .version('beta')
    .get();

```