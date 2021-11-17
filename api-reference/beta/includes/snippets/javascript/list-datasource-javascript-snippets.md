---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27223d31d54e9c37307dd4db9d0dd62ac0af99e58d1f28940134c4794ac49f8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216030"
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