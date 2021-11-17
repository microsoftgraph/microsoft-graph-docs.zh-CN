---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26fefb38a5dc6dbb1d98a6d008d59424f007a05e1b1818d5a4817f4126750e3d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161934"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userFlowIdentityProviders = await client.api('/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders')
    .version('beta')
    .get();

```