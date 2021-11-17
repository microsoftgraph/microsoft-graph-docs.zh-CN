---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1621ba892b7bc5b8d4633f4d5a1519789aecb9b8f9c2004ced84ddb649e005a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163228"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2')
    .version('beta')
    .delete();

```