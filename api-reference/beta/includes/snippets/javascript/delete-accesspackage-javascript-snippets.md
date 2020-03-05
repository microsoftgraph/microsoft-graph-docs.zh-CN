---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23c360e5057cf57c38a3eef128d58e0b945b84b5
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992908"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}')
    .version('beta')
    .delete();

```