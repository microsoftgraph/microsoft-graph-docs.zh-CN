---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd24c6eab992bc9b90b7eabd9f66c93358e77250
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780524"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let domain = await client.api('/domains/contoso.com')
    .version('beta')
    .get();

```