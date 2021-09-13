---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 780c29b71eb9c44adbd77cdc83fce61ae6635a209f8a9337bc3549b7ce17c612
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378846"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let administrativeUnit = await client.api('/education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/administrativeUnit')
    .get();

```