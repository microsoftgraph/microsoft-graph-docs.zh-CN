---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f3d3d5b644cf12c303294610de6086fbcad0e49
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996209"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/webAccounts/{id}')
    .version('beta')
    .delete();

```