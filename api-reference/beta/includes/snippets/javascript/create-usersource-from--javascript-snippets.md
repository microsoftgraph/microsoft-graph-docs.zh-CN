---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2c84b82fe09859054f732a7c7ecea53c652a273
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659000"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userSource = {
    email:"megan@contoso.com",
    includedSources:"mailbox, site"
};

let res = await client.api('/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources')
    .version('beta')
    .post(userSource);

```