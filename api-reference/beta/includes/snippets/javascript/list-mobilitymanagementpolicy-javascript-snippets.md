---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0d094e3718d8e9d7afd4bdd2a6a727b123685b1
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440882"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mobileAppManagementPolicies = await client.api('/policies/mobileAppManagementPolicies')
    .version('beta')
    .get();

```