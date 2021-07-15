---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34a797cadd4cf268d81a521e7d0d30957b6fdb84
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackagesIncompatibleWith = await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackagesIncompatibleWith')
    .version('beta')
    .get();

```