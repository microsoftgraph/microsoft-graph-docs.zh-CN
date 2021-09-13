---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b18f487bdb1835d599369c412c0c382a2ba3fe07849595c2d307dc5b3253850
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332548"
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
    .put(organizationalBranding);

```