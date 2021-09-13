---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5230b908c90af536ccd1575aa7d02f0a1e257665f9221ce042383dfdadf8c985
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279402"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/tokenLifetimePolicies/{id}/$ref')
    .delete();

```