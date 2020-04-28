---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b01c993375f40dbc1f8642ec39aec8713b7d4eb
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805383"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/tokenIssuancePolicies/{id}')
    .delete();

```