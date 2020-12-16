---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 630eae278a01dcae96bf47f93e95825c9f537f20
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690357"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .filter('distributionMethod eq 'organization'')
    .get();

```