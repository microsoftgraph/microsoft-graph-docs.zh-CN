---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b30138558e8ad2b0bf2301dbf1c564fb7d71b6f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803627"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{group-id}/members/{directory-object-id}/$ref')
    .delete();

```