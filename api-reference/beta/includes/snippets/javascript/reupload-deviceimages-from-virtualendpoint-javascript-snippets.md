---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 067bb91f629dd89f880bb10082b176851c8dc36faf36220cd2b5943fa0451fdc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162275"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/deviceManagement/virtualEndpoint/deviceImages/{cloudPcDeviceImageId}/reupload')
    .version('beta')
    .post();

```