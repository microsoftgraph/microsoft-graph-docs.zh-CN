---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 038d267d99c91a2551aa50a885a88a21f55f759cf7f32961bb2a0021adae2c05
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278134"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationContextClassReference = {
    id: 'c1',
    displayName: 'Contoso medium',
    description: 'Medium protection level defined for Contoso policy',
    isAvailable: true
};

await client.api('/identity/conditionalAccess/authenticationContextClassReferences')
    .version('beta')
    .post(authenticationContextClassReference);

```