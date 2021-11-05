---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 227f7ecb8bcd2acad9b015a5c2e5538068cb42e4
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60560439"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSubmissionResource = {
    resource: {
        '@odata.type': 'microsoft.graph.educationWordResource',
        displayName: 'Report.docx',
        fileUrl: 'https://graph.microsoft.com/v1.0/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2'
    }
};

await client.api('/education/classes/f4a941ff-9da6-4707-ba5b-0eae93cad0b4/assignments/3c77de7f-539b-49e1-9c96-1274f2f0ee3b/submissions/4af73d2b-6b9c-493f-0688-979087bed39b/resources')
    .post(educationSubmissionResource);

```