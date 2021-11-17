---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71d132e545be0be590ce2e6dbada2bdf4a4f098d13b218326c3c562a1cdee0af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333639"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const changePassword = {
    currentPassword: 'xWwvJ]6NMw+bWH-d',
    newPassword: '0eM85N54wFxWwvJ]'
};

await client.api('/me/changePassword')
    .version('beta')
    .post(changePassword);

```