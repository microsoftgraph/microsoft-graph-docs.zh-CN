---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30300193c9564bd49c68548fa8fb05bbf2dc87a2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  '@odata.type': 'microsoft.graph.mailSearchFolder',
  filterQuery: 'contains(subject, \'Analytics\')'
};

await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .version('beta')
    .update(mailFolder);

```