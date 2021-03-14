---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b013a3ba647abbe7f61d1da76de91d95c4ca54d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806692"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps')
    .expand('teamsAppDefinition')
    .get();

```