---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 252db7a585b1404e08d401ebde20c939491b35d5a9277516a7ab20c455b7c02a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162868"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleDefinitions = await client.api('/roleManagement/entitlementManagement/roleDefinitions')
    .version('beta')
    .get();

```