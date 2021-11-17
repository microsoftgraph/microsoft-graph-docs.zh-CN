---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a3a6cd34db0cf4637d85ee373d67a0546f45a44467e14deb381f3525a0016cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106659"
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