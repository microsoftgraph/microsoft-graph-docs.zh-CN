---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de00250784ffd78acf2aa862ed33a60bb4e9dc2c
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665335"
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