---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f5af704c913c533a3934fc246b3f6431a2b34a4
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921577"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby')
    .delete();

```