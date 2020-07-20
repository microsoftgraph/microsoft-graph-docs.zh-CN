---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bd5c2fc3bf82a86270c34410cac3f9c6048bd2f
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080717"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/organization/settings')
    .version('beta')
    .get();

```