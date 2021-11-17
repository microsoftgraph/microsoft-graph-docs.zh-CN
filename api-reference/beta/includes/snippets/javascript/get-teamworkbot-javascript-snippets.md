---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9edaceb31d94f7339f731e8cf62eb38fe775eb24340da0e743bca4343558d61a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163617"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamworkBot = await client.api('/appCatalogs/teamsApps/e4c5c249-bb4b-419e-b7c5-b1d98559368b/appDefinitions/ZTRjNWMyNDktYmI0Yi00MTllLWI3YzUtYjFkOTg1NTkzNjhiIyMyLjAuMSMjUHVibGlzaGVk/bot')
    .version('beta')
    .get();

```