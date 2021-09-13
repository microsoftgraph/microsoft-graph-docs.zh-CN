---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94b5965eb4a54b56643da8b34853901e5c09440c93ba05ad34fde54f6e3ca3f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378406"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamworkBot = await client.api('/appCatalogs/teamsApps/e4c5c249-bb4b-419e-b7c5-b1d98559368b/appDefinitions/ZTRjNWMyNDktYmI0Yi00MTllLWI3YzUtYjFkOTg1NTkzNjhiIyMyLjAuMSMjUHVibGlzaGVk/bot')
    .get();

```