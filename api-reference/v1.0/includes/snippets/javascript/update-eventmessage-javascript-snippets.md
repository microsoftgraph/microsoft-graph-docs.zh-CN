---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1296ef514fa6c7a23f600d334ead0bc0b17525d15071cae1668326b21f259890
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105560"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  isRead: true,
};

await client.api('/me/messages/{id}')
    .update(message);

```