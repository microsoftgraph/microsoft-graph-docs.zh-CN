---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ba84b4de89b063d7a2cb655f1db74b1fb086f149c05240716d1c729f016eb56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328770"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteSection = {
  displayName: 'Section name'
};

await client.api('/me/onenote/notebooks/{id}/sections')
    .version('beta')
    .post(onenoteSection);

```