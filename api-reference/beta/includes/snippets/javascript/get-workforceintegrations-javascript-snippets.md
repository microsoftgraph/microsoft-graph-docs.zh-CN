---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9e655ef561c1ec5e7b99881dc4625e4a165bde3
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "40870583"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teamwork/workforceIntegrations')
    .version('beta')
    .get();

```