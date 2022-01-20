---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b9106f810e52afa967eff9bb7a474c2daaf7ace
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128473"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let signIns = await client.api('/auditLogs/signIns?&$filter=startsWith(appDisplayName,\'Graph\')&top=10')
    .filter('startsWith(appDisplayName,\'Graph\')')
    .get();

```