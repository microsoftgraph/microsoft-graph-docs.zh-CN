---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c65f45bd2f5645c427cc6b4e32405d2de4f0689d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955791"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organizationalBranding = {
    backgroundColor: '#FFFF33',
    signInPageText: 'Welcome',
    usernameHintText: 'hint'
};

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding')
    .version('beta')
    .put(organizationalBranding);

```