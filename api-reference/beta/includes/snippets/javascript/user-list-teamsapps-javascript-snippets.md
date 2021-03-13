---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 598d2683a0b91bb00370582cfeb290632b0a3af5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788195"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/users/{id}/teamwork/installedApps')
    .version('beta')
    .get();

```