---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 973ce9228ae8e8814c8b3856faefbc4647dcd2241519d8b9bdc4ed9926dc50dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218955"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const changeScreenSharingRole = {
  role: 'viewer'
};

await client.api('/communications/calls/{id}/changeScreenSharingRole')
    .version('beta')
    .post(changeScreenSharingRole);

```