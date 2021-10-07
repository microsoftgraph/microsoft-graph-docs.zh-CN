---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cbd3e48b104c9c119b99727337f989c8f61fc8945d54fac0061d6ea21c46df2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219145"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email')
    .version('beta')
    .delete();

```