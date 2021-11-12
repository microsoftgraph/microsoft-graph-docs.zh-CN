---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b1f12d6067c40212911cd930970c4e2fd1eb1484bda38034eb3100452e5b83f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903067"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schedulingGroups = await client.api('/teams/{teamId}/schedule/schedulingGroups')
    .version('beta')
    .get();

```