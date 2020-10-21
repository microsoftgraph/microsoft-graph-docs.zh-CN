---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8507936454ad13a21c302b1f0700386b4a526eb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605169"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/subscriptions')
    .get();

```