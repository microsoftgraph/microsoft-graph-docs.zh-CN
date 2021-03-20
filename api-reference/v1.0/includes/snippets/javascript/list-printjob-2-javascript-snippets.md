---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcedeace0dfae1348e0b8f273af6249a834e88ce
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953425"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let jobs = await client.api('/print/shares/{printerShareId}/jobs')
    .get();

```