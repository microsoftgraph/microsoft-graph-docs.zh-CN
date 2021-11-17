---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f888145a08e7a67354436eca8d12e4181f934d93a6a5e9e96db7fe9612831200
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104782"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttribute = {
  displayName: 'Hobby',
  description: 'Your hobby',
  dataType: 'string',
};

await client.api('/identity/userFlowAttributes')
    .version('beta')
    .post(identityUserFlowAttribute);

```