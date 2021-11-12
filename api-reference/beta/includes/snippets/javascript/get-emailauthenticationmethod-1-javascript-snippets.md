---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 003dc5b2593a7bf15db70d6b059326674be420cdbb3d2ed0f573d9c2c164efae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163235"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let emailAuthenticationMethod = await client.api('/me/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f')
    .version('beta')
    .get();

```