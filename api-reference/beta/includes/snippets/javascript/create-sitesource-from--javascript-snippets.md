---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f282f9604776a84b6430a72b50c623185c27407f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773009"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const siteSource = {
    'site@odata.bind': 'https://graph.microsoft.com/v1.0/sites/50073f3e-cb22-48e5-95a9-51a3da455181'
};

await client.api('/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources')
    .version('beta')
    .post(siteSource);

```