---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b51f48827dde181ab2afac3266ab44914d91a66
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719268"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/tokenLifetimePolicies/{id}')
    .delete();

```