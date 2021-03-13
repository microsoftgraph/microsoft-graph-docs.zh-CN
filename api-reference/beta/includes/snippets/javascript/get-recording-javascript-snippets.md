---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22b7ad9a55567129d73f9e4c8cd8ab8503e3bbc2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785729"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/users/dc74d9bb-6afe-433d-8eaa-e39d80d3a647/onlineMeetings/dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw@thread.v2/recording')
    .version('beta')
    .get();

```