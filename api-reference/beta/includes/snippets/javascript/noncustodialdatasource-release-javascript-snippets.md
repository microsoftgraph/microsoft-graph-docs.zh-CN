---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d30641d3ea651e50f28087eca305867ef70c9e5ef564d0a62d3d19b17f44f578
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104809"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources/8e402dd7f3c94a3abc086e5d07db1c6d/release')
    .version('beta')
    .post();

```