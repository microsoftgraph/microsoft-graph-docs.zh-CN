---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16b300c6c309c80c1d01431f1ea2c30f97ac3679
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516123"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agreementFile = await client.api('/identityGovernance/termsOfUse/agreements/94410bbf-3d3e-4683-8149-f034e55c39dd/file')
    .get();

```