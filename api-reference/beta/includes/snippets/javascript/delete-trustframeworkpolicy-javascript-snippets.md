---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f5b6fb4ab5e2091b5b1cddaa5039d74ba75c23e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788023"
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