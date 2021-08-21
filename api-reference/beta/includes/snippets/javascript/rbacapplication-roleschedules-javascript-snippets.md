---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a0735dbd414374cc33f215b4ccdda94dd2f4886e8880da4e85709d7b5e5e1f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219926"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleSchedules = await client.api('/roleManagement/directory/roleSchedules(directoryScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',appScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',principalId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',roleDefinitionId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea')')
    .version('beta')
    .get();

```