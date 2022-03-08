---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db4025a6ccde1a4047147f5fe22560fdbc60c49c3464909d6d1f909d8af869b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164251"
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
    .version('beta')
    .post(removePassword);

```