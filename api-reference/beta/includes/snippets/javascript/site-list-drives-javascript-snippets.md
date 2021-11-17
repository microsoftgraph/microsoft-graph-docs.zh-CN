---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7e8933369806e8e57a559a610906b7c420b2e3daba6d71841dfcbbee61fe798
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105207"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/sites/{siteId}/drives')
    .version('beta')
    .get();

```