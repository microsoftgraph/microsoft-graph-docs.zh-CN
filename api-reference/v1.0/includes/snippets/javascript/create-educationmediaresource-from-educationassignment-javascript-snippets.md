---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c116126acd4fb61952bad7800269618b8f2a8eb
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60558730"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignmentResource = {
    distributeForStudentWork: false,
    resource: {
        '@odata.type': 'microsoft.graph.educationMediaResource',
        displayName: 'homework example.PNG',
        fileUrl: 'https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RMUWOKAGSJZ6BHINJVKNMOOJABF'
    }
};

await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources')
    .post(educationAssignmentResource);

```