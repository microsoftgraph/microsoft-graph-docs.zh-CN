---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78bc0fc1cbdfd2b18a84d45cddc4b5bb13865697
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819982"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('id eq '876df28f-2e78-423b-94a5-44181bd0e225',')
    .expand('appDefinitions')
    .get();

```