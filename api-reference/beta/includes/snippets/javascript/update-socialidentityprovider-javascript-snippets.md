---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b110e1bc9a22e7e38971b3a05a3e179d83e955cb
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviderBase = {
  clientSecret: '1111111111111'
};

await client.api('/identity/identityProviders/Amazon-OAUTH')
    .version('beta')
    .update(identityProviderBase);

```