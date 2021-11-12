---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fbf82cd5402ba8446e3382230b20ce25f5d440e5699e1088bc2ebf1e32c5555
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104068"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agreements = await client.api('/identityGovernance/termsOfUse/agreements')
    .version('beta')
    .get();

```