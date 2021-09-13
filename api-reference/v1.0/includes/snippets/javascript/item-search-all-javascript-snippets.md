---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f073ed4d3d331b9848cc72c7715e3bdaf627b2e2e3d42085a5e3025e44db892f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903342"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let search = await client.api('/me/drive/search(q='Contoso Project')')
    .get();

```