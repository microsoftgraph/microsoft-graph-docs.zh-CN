---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b0897fe2ba6b22fad7f0bf1febf8ad51c86fffe6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467026"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  @odata.type: "microsoft.graph.mailSearchFolder",
  displayName: "Weekly digests",
  includeNestedFolders: true,
  sourceFolderIds: ["AQMkADYAAAIBDAAAAA=="],
  filterQuery: "contains(subject, 'weekly digest')"
};

let res = await client.api('/me/mailfolders/AQMkADYAAAIBDAAAAA==/childfolders')
    .post({mailFolder : mailFolder});

```