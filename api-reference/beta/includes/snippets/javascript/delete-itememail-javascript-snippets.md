---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a62e69b521b0f06b468713766f05d2b1486ac295
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997381"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/emails/{id}')
    .version('beta')
    .delete();

```