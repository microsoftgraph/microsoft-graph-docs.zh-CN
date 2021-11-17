---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9713d33d5230db3d7e26ce9be7d62a86b9dd4aa5c13a9def24d21c5c2c3025d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277754"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let securityActions = await client.api('/security/securityActions')
    .version('beta')
    .get();

```