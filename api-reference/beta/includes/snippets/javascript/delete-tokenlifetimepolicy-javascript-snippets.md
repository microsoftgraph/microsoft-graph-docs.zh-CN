---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b427cf5278d0c2de174e954b613715f0dcdd46c8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780535"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/tokenLifetimePolicies/{id}')
    .version('beta')
    .delete();

```