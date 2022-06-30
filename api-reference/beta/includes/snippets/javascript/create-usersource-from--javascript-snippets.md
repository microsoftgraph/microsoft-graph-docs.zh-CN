---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fdf6967b0cd22e8ea3f748aeccdb7de8e7d9796
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438698"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userSource = {
    email: 'admin@M365x809305.onmicrosoft.com',
    includedSources: 'mailbox, site'
};

await client.api('/security/cases/ediscoveryCases/{ediscoveryCaseId}/legalHolds/{ediscoveryHoldPolicyId}/userSources')
    .version('beta')
    .post(userSource);

```