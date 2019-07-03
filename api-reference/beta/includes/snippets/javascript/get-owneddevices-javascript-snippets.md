---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f964c6b16ada4dad9d0ffd9b4ee99fdadf058b9b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521093"
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