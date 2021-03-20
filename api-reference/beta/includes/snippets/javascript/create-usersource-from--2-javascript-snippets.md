---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb518003a0281456780b6216814d0f7b57a14106
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userSource = {
  email: 'adelev@contoso.com',
  includedSources: 'mailbox'
};

await client.api('/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/userSources')
    .version('beta')
    .post(userSource);

```