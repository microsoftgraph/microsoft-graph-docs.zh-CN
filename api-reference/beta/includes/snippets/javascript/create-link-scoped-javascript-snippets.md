---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61393570191320e984864693f2bfe29a820c5cda
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619815"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: "edit",
  scope: "organization"
};

let res = await client.api('/me/drive/items/{item-id}/createLink')
    .version('beta')
    .post(permission);

```