---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 963bf06bb8adb037831a0d1c2fd7b5fd778bc485
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798196"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8')
    .version('beta')
    .delete();

```