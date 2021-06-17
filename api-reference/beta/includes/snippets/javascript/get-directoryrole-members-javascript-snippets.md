---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18227ecee8751736cfe843534983ba6dd68ca7f0
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990855"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda/members')
    .version('beta')
    .get();

```