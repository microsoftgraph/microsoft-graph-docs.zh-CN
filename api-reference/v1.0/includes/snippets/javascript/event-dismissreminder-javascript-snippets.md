---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ad4cb296e95947f0081d7c77059ab85e7a13cea1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510241"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}/dismissReminder')
    .post();

```