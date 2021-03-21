---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc3d64edcd6511827065bc9b18aee83748fcff9f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962322"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectors = await client.api('/print/connectors')
    .version('beta')
    .get();

```