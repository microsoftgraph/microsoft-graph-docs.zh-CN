---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cc864da3718fa322f6b1368f80774eba7700216
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212886"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let allowedMembers = await client.api('/teams/893075dd-2487-5634-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/sharedWithTeams/893075dd-2487-5634-925f-022c42e20265/allowedMembers')
    .version('beta')
    .get();

```