---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38c7e64171d2e001155a5ed301a507b4d757a0d0
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216796"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printIdentity = {
  @odata.id: "https://graph.microsoft.com/beta/groups/{id}"
};

let res = await client.api('/print/shares/{id}/allowedGroups/$ref')
    .version('beta')
    .post(printIdentity);

```