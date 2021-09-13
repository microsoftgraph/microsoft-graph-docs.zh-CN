---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f2e15896af9e32c7f471bcf4b04fdb1e23e97266ac7031d3e1b70a5283a5e10
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163519"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let policies = await client.api('/identity/conditionalAccess/policies')
    .get();

```