---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a311f2ea8559aaceef54aff01f03e8b557e9cee
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566889"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/settings')
    .version('beta')
    .get();

```