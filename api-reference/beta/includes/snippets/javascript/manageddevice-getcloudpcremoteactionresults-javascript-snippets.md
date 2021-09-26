---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c34ed725405d8a739b2da3958aa5f1b6698a5f8e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59766784"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getCloudPcRemoteActionResults = await client.api('/deviceManagement/managedDevices/{managedDeviceId}/getCloudPcRemoteActionResults')
    .version('beta')
    .get();

```