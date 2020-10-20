---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f964c6b16ada4dad9d0ffd9b4ee99fdadf058b9b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620005"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/ownedDevices')
    .version('beta')
    .get();

```