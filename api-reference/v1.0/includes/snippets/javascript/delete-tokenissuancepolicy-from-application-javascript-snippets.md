---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3ed666ef019235dfd32199a97709c2af92fbcf919ff6a686b53ca167aadb7a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279404"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/tokenIssuancePolicies/{id}/$ref')
    .delete();

```