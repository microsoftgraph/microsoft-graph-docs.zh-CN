---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2e557f4626415a0fa582d6aabe432eca8212d42083e02799ad430a26e940782
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161294"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removePassword = {
    keyId: 'f0b0b335-1d71-4883-8f98-567911bfdca6'
};

await client.api('/applications/{id}/removePassword')
    .version('beta')
    .post(removePassword);

```