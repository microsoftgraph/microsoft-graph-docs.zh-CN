---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dcd24f0ea8d4c00c5025ddde22964f65afd2b53c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466505"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  @odata.type: "microsoft.graph.mailSearchFolder",
  displayName: "Get MyAnalytics",
  includeNestedFolders: true,
  sourceFolderIDs: ["AAMkAGVmMDEzM"],
  filterQuery: "contains(subject, 'MyAnalytics')"
};

let res = await client.api('/me/mailFolders/searchfolders/childfolders')
    .version('beta')
    .post({mailFolder : mailFolder});

```