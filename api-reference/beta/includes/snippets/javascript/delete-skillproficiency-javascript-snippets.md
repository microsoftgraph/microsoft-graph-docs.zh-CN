---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc67ffaad333ce3a752e8875b3d74b36ccab6acd
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997522"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/skills/{id}')
    .version('beta')
    .delete();

```