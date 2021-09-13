---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be9a8ed6b3ddc035ea83580fd14fe470c0de334aaa3ca95a6ff50d168ffca8b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279414"
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

await client.api('/applications/{id}/addPassword')
    .post(passwordCredential);

```