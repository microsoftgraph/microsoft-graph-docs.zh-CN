---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0743eee67c61e0c669aa3319a9b575b1ebd49f1b
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516166"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let acceptances = await client.api('/identityGovernance/termsOfUse/agreements/94410bbf-3d3e-4683-8149-f034e55c39dd/acceptances')
    .version('beta')
    .get();

```