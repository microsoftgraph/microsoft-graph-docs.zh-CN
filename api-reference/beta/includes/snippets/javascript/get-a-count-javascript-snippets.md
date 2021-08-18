---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09d87f0156b55e18bd4eb03a519ad4d796bb7187
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368843"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/contacts')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .filter('startswith(displayName,\'A\')')
    .orderby('displayName')
    .top(1)
    .get();

```