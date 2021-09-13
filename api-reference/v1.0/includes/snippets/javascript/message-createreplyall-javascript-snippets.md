---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a322822af382101b2b8daf5f1aa63e838b9e83be1f0555a1c8d147f3eb6cce1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162975"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/messages/{id}/createReplyAll')
    .post();

```