---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae766fdd7deb4a36dd7870239ecd53e15244a3d1
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944902"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bitlocker/recoveryKeys')
    .version('beta')
    .header('ocp-client-name','"My Friendly Client"')
    .header('ocp-client-version','"1.2"')
    .filter('deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'')
    .get();

```