---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e6edc025adf449f3ca7fcab39d9ab2ce50865c6
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508916"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': ' https://graph.microsoft.com/beta/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da'
};

await client.api('/policies/featureRolloutPolicies/{id}/appliesTo/$ref')
    .version('beta')
    .post(directoryObject);

```