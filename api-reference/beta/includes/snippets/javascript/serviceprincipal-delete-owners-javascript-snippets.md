---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: e4f29fff9f05c30952de5c6f76aee41c16c15324
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49350409"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/owners/{id}/$ref')
    .delete();

```