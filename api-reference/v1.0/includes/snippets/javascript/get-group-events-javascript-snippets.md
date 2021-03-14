---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 990e6d61ce4b01d2cee89644fd44aa0e50467d44
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808215"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let events = await client.api('/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events')
    .get();

```