---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3ebcfd385fb5620db611e11d23cfd8f43498cb0e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479909"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProviders')
    .version('beta')
    .get();

```