---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50aeb75e9a919245db5b6967ad7eb66bfea8fbd4
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442832"
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