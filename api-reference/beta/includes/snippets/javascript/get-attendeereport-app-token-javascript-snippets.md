---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb443c7d10d6b159ad57ca651e003a32268fea9b1a81c14d0c37ddff61b6e31f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101381"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/users/dc74d9bb-6afe-433d-8eaa-e39d80d3a647/onlineMeetings/dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw@thread.v2/attendeeReport')
    .version('beta')
    .get();

```