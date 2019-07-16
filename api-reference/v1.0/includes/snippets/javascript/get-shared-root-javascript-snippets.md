---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b671bf8b62c13fbe580f84393749d24cbe8f78e0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736849"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/shares/{shareIdOrEncodedSharingUrl}')
    .get();

```