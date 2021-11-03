---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5aefd6d879a9b9d120823f179bb54509d5760d9
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695199"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let federatedIdentityCredential = await client.api('/applications/acd7c908-1c4d-4d48-93ee-ff38349a75c8/federatedIdentityCredentials/bdad0963-4a7a-43ae-b569-e67e1da3f2c0')
    .version('beta')
    .get();

```