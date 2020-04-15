---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c3c44d78adac9906b8018aec32e7ee26fda69d9
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2020
ms.locfileid: "43512243"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-title}')
    .version('beta')
    .get();

```