---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f85616c924a7959af5ea34df3a6648c2f0b495df
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59765050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .search('displayName:wa')
    .orderby('displayName')
    .get();

```