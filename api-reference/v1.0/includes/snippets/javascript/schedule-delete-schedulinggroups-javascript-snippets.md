---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b65318ceae4d23c55d9db425e02be91bb1efe4e19e9ad7b6cf01acdb758675c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215959"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}')
    .delete();

```