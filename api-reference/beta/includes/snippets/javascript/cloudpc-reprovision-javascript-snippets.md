---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d70dc23809ef342bf92cb9fe90c30ea7d457b3bd
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225098"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reprovision = {
  userAccountType: 'administrator',
  osVersion: 'windows10'
};

await client.api('/deviceManagement/virtualEndpoint/cloudPCs/4b5ad5e0-6a0b-4ffc-818d-36bb23cf4dbd/reprovision')
    .version('beta')
    .post(reprovision);

```