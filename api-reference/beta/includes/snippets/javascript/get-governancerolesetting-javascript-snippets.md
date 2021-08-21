---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06c84560038b4a78fcf9df9d2e6c38b471dd5a16c831074f02b4f2f98453a548
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903793"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let governanceRoleSetting = await client.api('/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9')
    .version('beta')
    .get();

```