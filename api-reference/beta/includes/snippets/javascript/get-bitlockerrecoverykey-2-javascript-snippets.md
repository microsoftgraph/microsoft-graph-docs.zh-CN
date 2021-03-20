---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 629cc89d5b3687f9484d45bc27a264f19be54921
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944344"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let recoveryKeys = await client.api('/informationProtection/bitlocker/recoveryKeys')
    .version('beta')
    .header('ocp-client-name','"My Friendly Client"')
    .header('ocp-client-version','"1.2"')
    .filter('deviceId eq \'1ab40ab2-32a8-4b00-b6b5-ba724e407de9\'')
    .get();

```