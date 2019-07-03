---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fa0bc3e12aa9f83df4af63b56bfde06b5cd5c5e7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35468000"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/installedApps')
    .expand('teamsAppDefinition')
    .get();

```