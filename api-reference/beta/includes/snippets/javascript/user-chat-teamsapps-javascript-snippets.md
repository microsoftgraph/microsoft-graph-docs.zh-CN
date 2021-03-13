---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c0de1195aa10e54f7ebd09a3ba6a2da139514fe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795094"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chat = await client.api('/users/f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c/teamwork/installedApps/ZjMyYjgzYmItNGZjOC00ZGI3LWI3ZjUtNzZjZGJiYjhhYTFjIyMyMmY3M2JiZS1mNjdhLTRkZWEtYmQ1NC01NGNhYzcxOGNiMmI=/chat')
    .version('beta')
    .get();

```