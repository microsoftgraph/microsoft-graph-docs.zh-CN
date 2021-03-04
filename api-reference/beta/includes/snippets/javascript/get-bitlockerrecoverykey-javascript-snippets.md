---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1dcbd4d5dd1cb25cccbe8a1e1419d8e7c9a5bf54
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437995"
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
    .filter('deviceId eq \'1ab40ab2-32a8-4b00-b6b5-ba724e407de9\'')
    .get();

```