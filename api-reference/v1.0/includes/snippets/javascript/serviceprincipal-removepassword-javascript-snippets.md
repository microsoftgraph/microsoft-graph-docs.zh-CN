---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a44024e607c5a84dce1de0de43f4bf21ed56604e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792413"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removePassword = {
    keyId: 'f0b0b335-1d71-4883-8f98-567911bfdca6'
};

await client.api('/servicePrincipals/{id}/removePassword')
    .post(removePassword);

```