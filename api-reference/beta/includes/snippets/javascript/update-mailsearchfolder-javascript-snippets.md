---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da4ac7b1a786c1fd526914175f2df21b574a05e5a6bfd9d0f3646258e43c1472
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274372"
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