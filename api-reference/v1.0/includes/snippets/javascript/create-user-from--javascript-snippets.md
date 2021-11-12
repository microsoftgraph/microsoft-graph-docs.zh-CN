---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63965eb7e5ca002e5f8bbd04382273b0035bf85649c313befb5060ba876db51c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162955"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/users/{userId}'
};

await client.api('/print/shares/{printerShareId}/allowedUsers/$ref')
    .post(user);

```