---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4ad98dd01c89a5540a518bf9e0162a292a158e436ddb25c62f9e073631031e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278402"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const checkin = {
  comment: 'Updating the latest guidelines'
};

await client.api('/drives/{drive-id}/items/{item-id}/checkin')
    .version('beta')
    .post(checkin);

```