---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b671bf8b62c13fbe580f84393749d24cbe8f78e0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467305"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/shares/{shareIdOrEncodedSharingUrl}')
    .get();

```