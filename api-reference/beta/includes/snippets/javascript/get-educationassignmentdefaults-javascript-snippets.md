---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3882ae2ade93041fe189cc080e2bdbec42593f4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470546"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{id}/assignmentDefaults')
    .version('beta')
    .get();

```