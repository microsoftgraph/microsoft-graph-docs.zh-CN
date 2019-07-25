---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9b1873653dc0e696c364b21c49fc85537c7ec4b0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895399"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/installedApps')
    .version('beta')
    .expand('teamsAppDefinition')
    .get();

```