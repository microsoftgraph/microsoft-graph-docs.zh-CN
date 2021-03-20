---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df7a3e99ca238ef640224be7c355a879c35f4e1b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944349"
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
    .get();

```