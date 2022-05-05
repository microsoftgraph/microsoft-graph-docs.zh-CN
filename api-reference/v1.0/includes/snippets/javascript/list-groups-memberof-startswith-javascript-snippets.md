---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 309a63a6e60adc7c02e94047acfbf428bd08cdb7
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209524"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/groups/{id}/memberOf/microsoft.graph.group')
    .header('ConsistencyLevel','eventual')
    .filter('startswith(displayName, \'A\')')
    .orderby('displayName')
    .get();

```