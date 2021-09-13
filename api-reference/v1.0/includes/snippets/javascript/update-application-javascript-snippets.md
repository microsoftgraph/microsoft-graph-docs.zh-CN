---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d4191aed2d7429f61a92124374863d358c9fc6b3b2aac406389fd2961b35672
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  displayName: 'New display name'
};

await client.api('/applications/{id}')
    .update(application);

```