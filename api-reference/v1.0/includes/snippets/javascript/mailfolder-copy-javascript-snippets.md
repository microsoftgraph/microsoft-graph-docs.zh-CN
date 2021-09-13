---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d601307cf7836bda0a5400ac40ba752777a358953c0838288ba4c4616c56d620
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221412"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  destinationId: 'destinationId-value'
};

await client.api('/me/mailFolders/{id}/copy')
    .post(mailFolder);

```