---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6992a35cb899ad9eff1f7128074ac816b680159099b7ca08bc6d094e6457c68
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278976"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviderBase = await client.api('/identity/identityProviders/MSASignup-OAUTH')
    .version('beta')
    .get();

```