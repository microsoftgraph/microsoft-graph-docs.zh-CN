---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4d3a28d4ca90ed6908d869d751940d8a18f13bd
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2021
ms.locfileid: "59766230"
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