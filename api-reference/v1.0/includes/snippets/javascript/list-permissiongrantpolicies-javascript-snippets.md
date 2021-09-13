---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45be5d1614854af0c3a8cae0277113dc2cb3a36a3d16c869172d65706fe09616
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissionGrantPolicies = await client.api('/policies/permissionGrantPolicies')
    .get();

```