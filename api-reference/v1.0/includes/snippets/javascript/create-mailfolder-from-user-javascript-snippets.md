---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cf73b72bfb1628f6a9ff1249a66f986edc6c31b4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723244"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: "displayName-value"
};

let res = await client.api('/me/mailFolders')
    .post({mailFolder : mailFolder});

```