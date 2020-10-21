---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 559344d7ebef9e7db480d8c05644d2cd1b951554
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617727"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education')
    .get();

```