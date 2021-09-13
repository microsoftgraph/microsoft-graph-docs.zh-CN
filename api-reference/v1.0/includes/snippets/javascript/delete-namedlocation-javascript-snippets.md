---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36f715eecaf587b6686838ba912049305bd2edf52bdd53cb0e23d9349d93949d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409508"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2')
    .delete();

```