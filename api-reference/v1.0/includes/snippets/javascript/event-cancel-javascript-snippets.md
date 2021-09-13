---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59a677c91d1bda61193620ba96b5468fdc2cba4745fa89b14afe348a27884d96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409567"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancel = {
  Comment: 'Cancelling for this week due to all hands'
};

await client.api('/me/events/{id}/cancel')
    .post(cancel);

```