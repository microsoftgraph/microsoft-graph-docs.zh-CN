---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c62dc4f8a56c88ddb68d201a63e83b048226011
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439479"
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