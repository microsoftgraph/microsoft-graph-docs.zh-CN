---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a0c3b8c773d617e438a951759f4d6e600d9721f
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805430"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/tokenIssuancepolicies/{id}')
    .get();

```