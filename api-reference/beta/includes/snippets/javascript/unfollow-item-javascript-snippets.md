---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc9e289fd051ad71346a7ddac4338bb06a63dc76
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776807"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{item-id}/unfollow')
    .version('beta')
    .delete();

```