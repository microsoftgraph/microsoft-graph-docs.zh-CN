---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 74d8efe099cf1a3d7f8fe5423a78577e1a7c5f68
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509875"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .select('displayName,givenName,postalCode')
    .get();

```