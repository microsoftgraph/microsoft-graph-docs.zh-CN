---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcedeace0dfae1348e0b8f273af6249a834e88ce
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771524"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let jobs = await client.api('/print/shares/{printerShareId}/jobs')
    .get();

```