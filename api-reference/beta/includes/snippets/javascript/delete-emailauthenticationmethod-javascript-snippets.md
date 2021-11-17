---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c6c249b9d1d08df8588904bb2e4c87cdd69eaaf658742f16523f988658a6ae3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163691"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f')
    .version('beta')
    .delete();

```