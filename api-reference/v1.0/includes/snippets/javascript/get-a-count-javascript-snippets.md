---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4d3a28d4ca90ed6908d869d751940d8a18f13bd
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368847"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/contacts')
    .header('ConsistencyLevel','eventual')
    .filter('startswith(displayName,\'A\')')
    .orderby('displayName')
    .top(1)
    .get();

```