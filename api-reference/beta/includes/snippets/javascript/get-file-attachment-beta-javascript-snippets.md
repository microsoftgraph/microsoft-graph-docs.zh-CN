---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4f26a368c6c0e54f4ec70b5caf657dab24b3f75734bd742ae2d94e543652eac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachment = await client.api('/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=')
    .version('beta')
    .get();

```