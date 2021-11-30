---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a33d7b36a6fd18d39bd7353f74c6fdf9ed3aea5bb45c7566a9621ff640f2c96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278452"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/disableSmsSignIn')
    .version('beta')
    .post();

```