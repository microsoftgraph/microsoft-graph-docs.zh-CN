---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f29fce5cf524e23712a596eaab3e2822b0a67308
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997702"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/projects/{id}')
    .version('beta')
    .delete();

```