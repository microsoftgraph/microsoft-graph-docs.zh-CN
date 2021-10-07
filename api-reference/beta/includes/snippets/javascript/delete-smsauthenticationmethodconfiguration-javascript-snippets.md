---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6fd71932fd6bd2bdc70fddec6221148cff15c3511772db041125e6c62b8d008
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279465"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms')
    .version('beta')
    .delete();

```