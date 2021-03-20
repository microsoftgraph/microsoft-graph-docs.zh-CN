---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e36d6ac311e7543daa0ea0420bbaeef153116c54
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956322"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectors = await client.api('/print/printers/{printerId}/connectors')
    .get();

```