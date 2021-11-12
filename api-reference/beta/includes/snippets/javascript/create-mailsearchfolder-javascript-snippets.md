---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03a1333149291ea74188f3af2e539b36e0c1a440cd9feefd1a54971a9f021fcf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278940"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  '@odata.type': 'microsoft.graph.mailSearchFolder',
  displayName: 'Weekly digests',
  includeNestedFolders: true,
  sourceFolderIds: ['AQMkADYAAAIBDAAAAA=='],
  filterQuery: 'contains(subject, \'weekly digest\')'
};

await client.api('/me/mailfolders/AQMkADYAAAIBDAAAAA==/childfolders')
    .version('beta')
    .post(mailFolder);

```