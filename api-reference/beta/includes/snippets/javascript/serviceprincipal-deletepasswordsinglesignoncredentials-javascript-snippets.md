---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3bf4e0e215863452467e4203146cbdfef6df966
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802215"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const deletePasswordSingleSignOnCredentials = {
  id: '5793aa3b-cca9-4794-679a240f8b58'
};

await client.api('/servicePrincipals/{id}/deletePasswordSingleSignOnCredentials')
    .version('beta')
    .post(deletePasswordSingleSignOnCredentials);

```