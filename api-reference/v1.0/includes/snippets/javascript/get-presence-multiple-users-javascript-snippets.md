---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 881f16971f17f9a9d44782a46687d429123a6a7a35300ca0aa3b3d3ef02dba12
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903367"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const presence = {
    ids: ['fa8bf3dc-eca7-46b7-bad1-db199b62afc3', '66825e03-7ef5-42da-9069-724602c31f6b']
};

await client.api('/communications/getPresencesByUserId')
    .post(presence);

```