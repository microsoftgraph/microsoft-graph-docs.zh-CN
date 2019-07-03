---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d456ab2c81247fea29c216bf3053d14a9afe4cb3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478490"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null')
    .version('beta')
    .filter('siteCollection/root ne null')
    .get();

```