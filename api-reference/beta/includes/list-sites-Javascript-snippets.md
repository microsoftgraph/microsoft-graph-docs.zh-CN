---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d456ab2c81247fea29c216bf3053d14a9afe4cb3
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536951"
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