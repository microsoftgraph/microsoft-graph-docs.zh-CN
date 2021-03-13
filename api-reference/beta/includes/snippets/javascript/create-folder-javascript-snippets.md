---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df1eb6225557eea20f78c86aa5b23c713c53c0d7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781394"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: 'New Folder',
  folder: { },
  '@microsoft.graph.conflictBehavior': 'rename'
};

await client.api('/me/drive/root/children')
    .version('beta')
    .post(driveItem);

```