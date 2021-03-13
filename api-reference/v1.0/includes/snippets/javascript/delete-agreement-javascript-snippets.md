---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 278ef057bc432562c9b9f1f69a1be501d6d24eae
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768911"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be')
    .delete();

```