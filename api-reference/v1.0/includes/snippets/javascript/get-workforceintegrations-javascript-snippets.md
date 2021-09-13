---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2aeb33f259e27e052b52fd67a558488216204284f775e7f6735802df7ca7ffb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333900"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workforceIntegrations = await client.api('/teamwork/workforceIntegrations')
    .get();

```