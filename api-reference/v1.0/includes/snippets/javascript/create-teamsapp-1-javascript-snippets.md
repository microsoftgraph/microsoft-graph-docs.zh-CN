---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78c2a67e3d7631cfd2131d35e68188e3d29a556732a3f92d9ce125158b17e791
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219876"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsApp = [Zip file containing a Teams app package];

await client.api('/appCatalogs/teamsApps')
    .post(teamsApp);

```