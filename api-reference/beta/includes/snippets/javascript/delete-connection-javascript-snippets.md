---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d128b45bd1ea1d6b85362022faba5dd1cdb003f1
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994689"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/connections/contosohr')
    .version('beta')
    .delete();

```