---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c6ee3fd3c0f6b51345cc9bbf3b3c9ad915f98f9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806602"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk/upgrade')
    .post();

```