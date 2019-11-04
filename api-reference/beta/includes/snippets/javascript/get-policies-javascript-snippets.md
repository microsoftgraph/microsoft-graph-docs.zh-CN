---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4f55d0ef9e90c74c5903f6b128b522cf2dc016a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936653"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/conditionalAccess/policies')
    .version('beta')
    .filter('displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'')
    .get();

```