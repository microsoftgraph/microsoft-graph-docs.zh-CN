---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bec5af686743da7702d27d1f62a07a5e94c62ef
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766196"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignmentSettings = await client.api('/education/classes/f4a941ff-9da6-4707-ba5b-0eae93cad0b4/assignmentsettings')
    .get();

```