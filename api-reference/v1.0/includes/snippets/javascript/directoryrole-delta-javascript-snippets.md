---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c7b229a0b437320d505aa1ed445bc6b29ae58cf
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603890"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/delta')
    .get();

```