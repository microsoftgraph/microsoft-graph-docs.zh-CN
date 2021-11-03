---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efacd086941328bcf8b6f6966b4e804d97288027
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60690103"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/bcd7c908-1c4d-4d48-93ee-ff38349a75c8/federatedIdentityCredentials/d9b7bf1e-429e-4678-8132-9b00c9846cc4')
    .version('beta')
    .delete();

```