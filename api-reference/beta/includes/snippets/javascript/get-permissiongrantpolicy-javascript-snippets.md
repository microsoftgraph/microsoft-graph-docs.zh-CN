---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f648076c4290dc1f08034e6c19ceb65d54065a9c544d72b1b79bbe9e556833f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278927"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissionGrantPolicy = await client.api('/policies/permissionGrantPolicies/microsoft-user-default-low')
    .version('beta')
    .get();

```