---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32c9ada16161d61dd09089d21a4f0f6a455b7dbad1ab5518d10fd0566497e849
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221357"
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