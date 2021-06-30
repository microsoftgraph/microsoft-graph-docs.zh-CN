---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f870108935006948352114715bf80b6d0cc2d26
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedMembers = await client.api('/directoryRoles/roleTemplateId=fdd7a751-b60b-444a-984c-02652fe8fa1c/scopedMembers')
    .version('beta')
    .get();

```