---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cd6c5e98527fbae5a764f9672bc86f9ee103027
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961470"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectors = await client.api('/print/printers/{id}/connectors')
    .version('beta')
    .get();

```