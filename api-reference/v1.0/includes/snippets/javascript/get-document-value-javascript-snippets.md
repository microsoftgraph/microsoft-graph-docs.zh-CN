---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 761c15bca97feea96023712c40a0f6a235c34043
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772091"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/$value')
    .get();

```