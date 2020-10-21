---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1d8a68f7a35f534d32302a585267269ab3d6d18
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603515"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events')
    .get();

```