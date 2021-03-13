---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 630312cb5b62bac6c06ced0d7217b8d013337daf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775988"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printJob = await client.api('/print/printers/{printerId}/jobs/{printJobId}')
    .get();

```