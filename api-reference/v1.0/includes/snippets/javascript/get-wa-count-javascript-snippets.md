---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63de74e7d45bb302289b9e19f2c1e593e1740856
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764409"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .header('ConsistencyLevel','eventual')
    .search('displayName:wa')
    .orderby('displayName')
    .get();

```