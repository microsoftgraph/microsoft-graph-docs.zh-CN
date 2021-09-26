---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f70ebb328bc3412bd51d520a122a2b58a204ce43785a04b1f288290484da935b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158381"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcUserSetting = await client.api('/deviceManagement/virtualEndpoint/userSettings/556092f8-92f8-5560-f892-6055f8926055')
    .version('beta')
    .get();

```