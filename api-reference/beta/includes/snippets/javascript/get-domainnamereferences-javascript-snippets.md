---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 300aa93262e375366c3b9a400fb9f63c4c3c8874
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500600"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com/domainNameReferences')
    .version('beta')
    .get();

```