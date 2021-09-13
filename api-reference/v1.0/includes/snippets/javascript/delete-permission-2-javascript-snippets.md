---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 384a79daaf39cd599a82bb97202bb391b64cff888f1683c18aed8734125419c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333343"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .delete();

```