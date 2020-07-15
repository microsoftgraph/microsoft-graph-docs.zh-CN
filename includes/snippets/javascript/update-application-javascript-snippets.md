---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be0314925c59638a698a655917e7defb7c42197e
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142322"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
   onPremisesPublishing: {
      singleSignOnSettings: {
         kerberosSignOnSettings: {
            kerberosServicePrincipalName: "HTTP/iwademo.contoso.com",
        kerberosSignOnMappingAttributeType: "userPrincipalName"
         },
         singleSignOnMode: "onPremisesKerberos"
      }
   }
};

let res = await client.api('/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83')
    .version('beta')
    .update(application);

```