---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc7d37f2884745f6087d23ab5c4e6126b38ba67e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022497"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let externalGroup = await client.api('/external/connections/contosohr/groups/31bea3d537902000')
    .get();

```