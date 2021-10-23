---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05b562c3532b18ad82eb9a8548a7f03b93ed2204
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559871"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let caseSettings = await client.api('/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/settings')
    .version('beta')
    .get();

```