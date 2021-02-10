---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 398e60120e8b138edcabe1fb34ea50fe97e62149
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50178968"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/roleManagement/deviceManagement/roleAssignments')
    .version('beta')
    .get();

```