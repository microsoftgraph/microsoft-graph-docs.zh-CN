---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29edc0e2d1bd1b15ac561be236c8d0a92336fbcdc736129ac3ffdfe8dc5f972e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162603"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directoryRoles/f8e85ed8-f66f-4058-b170-3efae8b9c6e5/members/bb165b45-151c-4cf6-9911-cd7188912848/$ref')
    .delete();

```