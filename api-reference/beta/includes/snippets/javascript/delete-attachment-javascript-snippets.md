---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07040a2c2ccc345299018f3633e246f311cfcec21b1d70b485318cc78192d7d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902915"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/events/{id}/attachments/{id}')
    .version('beta')
    .delete();

```