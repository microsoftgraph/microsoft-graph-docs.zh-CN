---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8020a38aaea6c6c799f81d8a105f64c229a1778
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997085"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/websites/{id}')
    .version('beta')
    .delete();

```