---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69d7554a09fc2f3e586a6b27a6e6a9433818dd48
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2020
ms.locfileid: "46657972"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getM365AppUserCounts(period='D7')/content')
    .version('beta')
    .get();

```