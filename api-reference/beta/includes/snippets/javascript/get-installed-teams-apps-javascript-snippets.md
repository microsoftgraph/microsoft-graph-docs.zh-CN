---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17c3d61f209aab6db96c19ad8c2b101004b7a56939103947a8a46806c216bcc9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106257"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsAppInstallation = await client.api('/teams/{id}/installedApps/{id}')
    .version('beta')
    .get();

```