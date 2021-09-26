---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9b88f5422d5fa9bdd8e6cdea9df9b9bacf4251ab17264cd0fe7d1de8bebfc01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902472"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleDefinition = await client.api('/roleManagement/cloudPC/roleDefinitions/d40368cb-fbf4-4965-bbc1-f17b3a78e510')
    .version('beta')
    .get();

```