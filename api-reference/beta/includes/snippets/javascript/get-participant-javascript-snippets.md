---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab83fe19a0470da62ab544109f5e824b56441804d5a2567b96bec628cd771ab3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274351"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let participant = await client.api('/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/7e1b4346-85a6-4bdd-abe3-d11c5d420efe')
    .version('beta')
    .get();

```