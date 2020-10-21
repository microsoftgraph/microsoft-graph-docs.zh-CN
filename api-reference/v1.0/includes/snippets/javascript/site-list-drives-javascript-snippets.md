---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a43575cee0bf173082f1e67664df9e3dfa43d2e8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606819"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{siteId}/drives')
    .get();

```