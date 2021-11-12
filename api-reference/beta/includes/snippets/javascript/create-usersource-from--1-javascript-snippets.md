---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ec010f7753fac7ab1371a7ca5232234c2ddc546886c249370ba551a10bbd08c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161502"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userSource = {
    email: 'megan@contoso.com',
    includedSources: 'mailbox, site'
};

await client.api('/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources')
    .version('beta')
    .post(userSource);

```