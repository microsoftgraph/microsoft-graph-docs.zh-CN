---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6ed4e11508d429e42cf86dfdbb211f75b5cabac
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805854"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityProviders/Amazon-OAuth')
    .delete();

```