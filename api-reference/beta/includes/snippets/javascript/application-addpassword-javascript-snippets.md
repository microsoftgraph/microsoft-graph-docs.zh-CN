---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a7d25d353538b847760605ce7f2e4356df9213f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37995590"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const passwordCredential = {
  passwordCredential: {
    displayName: "Password friendly name"
  }
};

let res = await client.api('/applications/{id}/addPassword')
    .version('beta')
    .post(passwordCredential);

```