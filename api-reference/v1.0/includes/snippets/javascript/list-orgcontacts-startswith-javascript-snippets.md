---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4d3a28d4ca90ed6908d869d751940d8a18f13bd
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207733"
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