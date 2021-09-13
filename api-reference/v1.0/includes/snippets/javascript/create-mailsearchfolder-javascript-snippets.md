---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a718e0e9332a46714a36eaa02961fd42502a1ab4c56aefa77e0817c58c5bb08b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274051"
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
    .post(mailFolder);

```