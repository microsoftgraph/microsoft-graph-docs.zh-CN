---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df2fc34ae82d724d58a5529dfbec0c4c3d6a4d64
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783618"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const linkedResource = {
  '@odata.type': '#microsoft.graph.linkedResource',
  webUrl: 'http://microsoft.com',
  applicationName: 'Microsoft',
  displayName: 'Microsoft'
};

await client.api('/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9')
    .update(linkedResource);

```