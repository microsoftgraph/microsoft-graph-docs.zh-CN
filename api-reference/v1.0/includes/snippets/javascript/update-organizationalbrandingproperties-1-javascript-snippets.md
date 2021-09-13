---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9c6404aa64d844fe40caa99ef39b97a5a05431b272b8cc99d063cfe7969b596
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56831188"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organizationalBranding = {
    signInPageText: 'Default',
    usernameHintText: 'DefaultHint'
};

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding')
    .update(organizationalBranding);

```