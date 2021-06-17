---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7caeef3119ec2587abf88f57d68f031decd439fd
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991742"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRole = await client.api('/directoryRoles/fe8f10bf-c9c2-47eb-95cb-c26cc85f1830')
    .version('beta')
    .get();

```