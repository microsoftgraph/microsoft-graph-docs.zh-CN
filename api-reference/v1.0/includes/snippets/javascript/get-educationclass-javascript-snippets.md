---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48affcc5fd08d8d00cfc8ed6af4de33b740f16e3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778117"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationClass = await client.api('/education/classes/{class-id}')
    .get();

```