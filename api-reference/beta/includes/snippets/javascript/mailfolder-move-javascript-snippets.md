---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59179c4702550f56e91fc4a476fedc2453a01d946f135eac96db88342284dfe4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106526"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  destinationId: 'destinationId-value'
};

await client.api('/me/mailFolders/{id}/move')
    .version('beta')
    .post(mailFolder);

```