---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5115bd075303bd0bef2ab0d2df3b180c485d5384
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771020"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}')
    .version('beta')
    .delete();

```