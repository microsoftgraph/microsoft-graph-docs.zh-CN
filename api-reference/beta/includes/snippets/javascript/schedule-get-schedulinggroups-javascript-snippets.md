---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cbf5c24df99d0b418bb625eae6adccfb3a7c86255cdaf8f800898b3b20df06a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103841"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schedulingGroup = await client.api('/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}')
    .version('beta')
    .get();

```