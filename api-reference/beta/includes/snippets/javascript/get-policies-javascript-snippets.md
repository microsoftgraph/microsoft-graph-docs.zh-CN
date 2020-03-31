---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8de11828fd6a46e5c6d9ace4e705f8b1071e40fe
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062392"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/conditionalAccess/policies')
    .version('beta')
    .filter('displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'')
    .get();

```