---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e37f142f2f656ae9054246dd033284a28bc7d32277de53cf3c293e00f727f24
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163676"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/kim@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2')
    .version('beta')
    .delete();

```