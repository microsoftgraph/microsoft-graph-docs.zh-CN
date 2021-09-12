---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbfb3287073b58f4742051e6ae9992b2a9465426cb2005800c39b04bd77b6d79
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218642"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/users/{id | userPrincipalName}')
    .select('displayName,givenName,postalCode')
    .get();

```