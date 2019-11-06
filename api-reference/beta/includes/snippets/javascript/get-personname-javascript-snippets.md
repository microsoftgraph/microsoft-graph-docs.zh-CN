---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6239fbdace404d3ae24431cf17d0d7dec1161f77
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998073"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/names/{id}')
    .version('beta')
    .get();

```