---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bfc03e8db6f40e0eb4b31c9124c19550d796d43
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177163"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .version('beta')
    .delete();

```