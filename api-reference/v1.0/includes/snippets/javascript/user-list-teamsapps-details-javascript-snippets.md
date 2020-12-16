---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bacd536603ba6bc252e083ebd44bedcdb0c0767
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690944"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps')
    .expand('teamsAppDefinition')
    .get();

```