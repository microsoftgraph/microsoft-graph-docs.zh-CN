---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f45b60b7df79e2d800af8082bedb9d94437e633
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991750"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directoryRoles/f8e85ed8-f66f-4058-b170-3efae8b9c6e5/members/bb165b45-151c-4cf6-9911-cd7188912848/$ref')
    .version('beta')
    .delete();

```