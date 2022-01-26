---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c948d4f8f479a27adeb5c45148c239e6722ba199
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225013"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcOrganizationSettings = {
  '@odata.type': '#microsoft.graph.cloudPcOrganizationSettings',
  userAccountType: 'standardUser',
  osVersion: 'windows11'
};

await client.api('/deviceManagement/virtualEndpoint/organizationSettings')
    .version('beta')
    .update(cloudPcOrganizationSettings);

```