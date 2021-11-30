---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efcfe2f721d561303669edcdf7d1103fcac4736d4de9b1e9d425f3b38e9431c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279111"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword')
    .version('beta')
    .post();

```