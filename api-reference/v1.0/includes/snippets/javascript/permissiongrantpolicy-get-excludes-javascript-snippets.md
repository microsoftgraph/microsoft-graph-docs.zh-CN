---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f91d73c6dda93f3dfd5ff8d58fe312b5a24964860cacb558360211d3193be79c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220978"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let excludes = await client.api('/policies/permissionGrantPolicies/microsoft-application-admin/excludes')
    .get();

```