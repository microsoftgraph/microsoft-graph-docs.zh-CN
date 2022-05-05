---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7476cb5ad43b8a0335000c520fc0b6d14e746a2e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204583"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rules = await client.api('/policies/roleManagementPolicies/DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448/rules')
    .get();

```