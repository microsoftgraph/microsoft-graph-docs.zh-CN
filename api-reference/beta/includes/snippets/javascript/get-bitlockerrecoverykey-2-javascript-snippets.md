---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cf45881db1ae4b717ddcedbf00f0e96813ad87a82a4ce2e9194085e5e9bdf47
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105868"
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