---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 02ad49ae46ec2b7a831afe4906a5d0a411c04434
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636724"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  @odata.type: "microsoft.graph.mailSearchFolder",
  filterQuery: "contains(subject, 'Analytics')"
};

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .version('beta')
    .update(mailFolder);

```