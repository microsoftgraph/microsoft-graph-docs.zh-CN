---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4af172a1a4246be1c5de5583829ec3c6e9a623977705c35c08761dffc10f68ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409502"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy/excludes/6a846635-3e70-4a10-821e-512a0db93cbd')
    .delete();

```