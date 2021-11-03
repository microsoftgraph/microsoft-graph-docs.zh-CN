---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 971fcb3d05ff0f34c058959be6a1f88e04806b80
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730366"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let recoveryKeys = await client.api('/informationProtection/bitlocker/recoveryKeys')
    .header('ocp-client-name','"My Friendly Client"')
    .header('ocp-client-version','"1.2"')
    .filter('deviceId eq \'1ab40ab2-32a8-4b00-b6b5-ba724e407de9\'')
    .get();

```