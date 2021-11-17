---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b75aaabe042e9e159f507825b6227dc775024fa925a328d5dbab0cdd9bb1f8de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161597"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const applicationServicePrincipal = {
  displayName: 'My custom name'
};

await client.api('/applicationTemplates/{id}/instantiate')
    .version('beta')
    .post(applicationServicePrincipal);

```