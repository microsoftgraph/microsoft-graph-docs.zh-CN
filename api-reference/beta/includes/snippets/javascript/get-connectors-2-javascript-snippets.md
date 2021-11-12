---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3d9a24267c1eb6f7911b440e2cbedeb57e266f1ecc3839bd07d36bc0959884d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220080"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectors = await client.api('/print/connectors')
    .version('beta')
    .get();

```