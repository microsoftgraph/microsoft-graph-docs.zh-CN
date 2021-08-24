---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72f49bea424a7c1c7e8eb77c6608ee18f9c9c3ac7c10653cb6e77952c8b00aed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334081"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const passwordCredential = {
  passwordCredential: {
    displayName: 'Password friendly name'
  }
};

await client.api('/servicePrincipals/{id}/addPassword')
    .post(passwordCredential);

```