---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7b2d7dba1354d1e65b6c92dd44d247b68c5e805
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689225"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const federatedIdentityCredential = {
    name: 'testing02',
    issuer: 'https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0',
    subject: 'a7d388c3-5e3f-4959-ac7d-786b3383006a',
    audiences: [
        'api://AzureADTokenExchange'
    ]
};

await client.api('/applications/bcd7c908-1c4d-4d48-93ee-ff38349a75c8/federatedIdentityCredentials/')
    .version('beta')
    .post(federatedIdentityCredential);

```