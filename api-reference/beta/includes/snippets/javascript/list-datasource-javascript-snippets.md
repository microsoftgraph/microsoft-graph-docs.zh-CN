---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34c11648f3ed0aaa5251387f603d651e2a8c8adc
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239600"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let dataSource = await client.api('/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources/8e402dd7f3c94a3abc086e5d07db1c6d/datasource')
    .version('beta')
    .get();

```