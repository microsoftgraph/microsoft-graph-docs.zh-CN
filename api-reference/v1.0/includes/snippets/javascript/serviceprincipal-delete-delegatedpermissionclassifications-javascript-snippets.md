---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 090d66d21ddf79daf11a7e5e1caeef30b91b6e73c952e7f17efdbb2df07267a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/delegatedPermissionClassifications/{id}')
    .delete();

```