---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f64b754adc996b1c779c1e5250d77116e77efbefe40d9b515c45bc728c2735b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278275"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodConfiguration = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms')
    .version('beta')
    .get();

```