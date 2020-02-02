---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b63f1e8b455f300ee438f6568cf4d499fc072f41
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636821"
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
    .post(mailFolder);

```