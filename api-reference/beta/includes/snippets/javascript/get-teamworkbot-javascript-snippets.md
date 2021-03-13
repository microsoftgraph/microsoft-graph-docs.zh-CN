---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd2fd8f05d55c8b502bc93b080141803328b26ab
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796108"
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