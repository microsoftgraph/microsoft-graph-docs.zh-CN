---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93832f79006af6e8737b990401871f6a246775c5
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591717"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/tokenIssuancepolicies/{id}')
    .version('beta')
    .get();

```