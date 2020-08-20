---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ef12b5c32cbc10aa7e87297e7e12072268e7c8b
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819954"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/publications')
    .version('beta')
    .get();

```