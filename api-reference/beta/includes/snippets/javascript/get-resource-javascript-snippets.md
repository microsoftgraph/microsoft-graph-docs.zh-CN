---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a597b589eb11940207af57e7efa5d79998342b367e7c125343245c178ffe8a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161541"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/me/onenote/resources/{id}/content')
    .version('beta')
    .get();

```