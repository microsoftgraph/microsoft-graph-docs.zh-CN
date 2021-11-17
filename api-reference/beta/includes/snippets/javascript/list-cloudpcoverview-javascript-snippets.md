---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8834058482f5ed7004584704e67301b06baeee88835c62c545721e07347536fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103989"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcsOverview = await client.api('/tenantRelationships/managedTenants/cloudPcsOverview')
    .version('beta')
    .get();

```