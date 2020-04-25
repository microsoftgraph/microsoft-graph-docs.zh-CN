---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36358f4af136445563b91d2aa31a78ffc1708e4e
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806675"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/tokenIssuancePolicies/{id}/$ref')
    .delete();

```