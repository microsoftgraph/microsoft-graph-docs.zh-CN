---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fb94600a5657edb9b7753921d76a96bb956c14c
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441551"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let aggregatedPolicyCompliances = await client.api('/tenantRelationships/managedTenants/aggregatedPolicyCompliances')
    .version('beta')
    .get();

```