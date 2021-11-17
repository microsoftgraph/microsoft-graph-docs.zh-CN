---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 910065e5aa98d02515ba5f5fabf542f73fdbe830f26617b3479b301e3e975de7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105525"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let controls = await client.api('/programs/673a7379-9c38-4f01-bd9d-4fda7260b807/controls')
    .version('beta')
    .get();

```