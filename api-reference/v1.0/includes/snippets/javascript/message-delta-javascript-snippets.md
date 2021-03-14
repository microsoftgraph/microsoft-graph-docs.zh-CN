---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d2c76d75544452ae656752f0b9f8f0c39c56f9c3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789975"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/mailFolders/{id}/messages/delta')
    .header('Prefer','odata.maxpagesize=2')
    .get();

```