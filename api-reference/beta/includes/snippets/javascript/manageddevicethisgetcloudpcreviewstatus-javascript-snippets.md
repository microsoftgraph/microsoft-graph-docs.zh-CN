---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 978f76cb952667c6f0aebd1c9dc0f005f918f7cd
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcReviewStatus = await client.api('/deviceManagement/managedDevices/185f01c2de954929afb129392e5d9f47/getCloudPcReviewStatus')
    .version('beta')
    .get();

```