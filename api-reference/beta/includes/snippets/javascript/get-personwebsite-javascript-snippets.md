---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9075156a9d6951603d3355e0931a6c2e74be41e
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997183"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/websites/{id}')
    .version('beta')
    .get();

```