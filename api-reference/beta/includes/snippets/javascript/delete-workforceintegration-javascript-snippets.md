---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a6a9bdfaf03c49586cb05f39ad674a61c325b77
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870515"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teamwork/workforceIntegrations')
    .version('beta')
    .delete();

```