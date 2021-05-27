---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7eec8f5432fbb0cd3862ff4f4e6ac863b330947b
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668678"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/identityProviders/{id}')
    .version('beta')
    .delete();

```