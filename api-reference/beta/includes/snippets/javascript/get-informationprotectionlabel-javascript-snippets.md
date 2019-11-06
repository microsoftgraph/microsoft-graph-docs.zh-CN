---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4080b45826259175a9a0e7d8b893c2b30886a60
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995646"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/informationprotection/policy/labels/{id}')
    .version('beta')
    .get();

```