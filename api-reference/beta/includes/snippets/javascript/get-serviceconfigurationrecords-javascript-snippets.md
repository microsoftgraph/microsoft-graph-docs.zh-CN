---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e80a2e3ff0c3d827d39020ab6aecd04bfa1f38c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com/serviceConfigurationRecords')
    .version('beta')
    .get();

```