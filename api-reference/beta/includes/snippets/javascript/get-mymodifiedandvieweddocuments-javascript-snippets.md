---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 002bb7c3395cf1572934697d2ee1c78c9dc80a47
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873969"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/insights/used')
    .version('beta')
    .orderby('LastUsed/LastAccessedDateTime desc')
    .get();

```