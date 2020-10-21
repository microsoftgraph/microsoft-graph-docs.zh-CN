---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c57e7d4a27e35fcad471fa98528b2ef044efa4cb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618124"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles')
    .get();

```