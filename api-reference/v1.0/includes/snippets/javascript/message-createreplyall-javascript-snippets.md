---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 055ad830aec3f7245be098bc8f2715a4c3ffd2a2
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "35732169"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/createReplyAll')
    .post();

```