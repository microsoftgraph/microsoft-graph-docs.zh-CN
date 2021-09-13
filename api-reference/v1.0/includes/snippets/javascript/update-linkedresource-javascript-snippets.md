---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b1f5aa6b949bec1be12dedc343db229a17e4db105032e2f904ac469431940b7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277511"
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