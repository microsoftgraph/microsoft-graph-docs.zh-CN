---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39da17f8b0f6526f6703ea348a3eaec020b6e68278ecfe4a4bcb44c3169f609f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903274"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignmentSchedules = await client.api('/roleManagement/directory/roleAssignmentSchedules')
    .version('beta')
    .get();

```