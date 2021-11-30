---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df55b5b4a4640314a4aaff38f5de686aab6e6dac66216c624d887295a53e1a22
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274344"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/enableSmsSignIn')
    .version('beta')
    .post();

```