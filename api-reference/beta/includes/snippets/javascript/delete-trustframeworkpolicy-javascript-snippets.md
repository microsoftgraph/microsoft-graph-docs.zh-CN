---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e45fdbc5afdbc3e409ad55881686e2d420e3c29a60f11d38b6a5bffc70beae42
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163335"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base')
    .version('beta')
    .delete();

```