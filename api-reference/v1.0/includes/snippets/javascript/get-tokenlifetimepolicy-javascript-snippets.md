---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f87e941f0543ce13d4236625a3af06ffefd9007
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719233"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/tokenLifetimePolicies/{id}')
    .get();

```