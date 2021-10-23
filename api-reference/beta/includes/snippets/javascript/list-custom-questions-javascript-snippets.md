---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcbdb31defdfdb95b848e8ae2130de9bd768f13d
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561224"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let customQuestions = await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/customQuestions')
    .version('beta')
    .get();

```