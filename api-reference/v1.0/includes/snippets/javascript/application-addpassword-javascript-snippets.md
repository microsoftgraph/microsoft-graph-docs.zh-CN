---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39b1b4e191ba1f9b270f5e2e0ac6b0b80a3bae26
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37999433"
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
    .post(passwordCredential);

```