---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6a607592901cd6e7c5e9f022f707fcbe0ee63f9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810543"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let webAccount = await client.api('/me/profile/webAccounts/{id}')
    .version('beta')
    .get();

```