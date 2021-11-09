---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6751dac0667155f82e890e8452e66c9b16f5f03b
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60560882"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSubmissionResource = {
    resource: {
        '@odata.type': '#microsoft.graph.educationExcelResource',
        displayName: 'userAgeGroup QueryParameter Test.xlsx',
        fileUrl: 'https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RONPUDM2CZKNRF3TGHYUM7Z64WE'
    }
};

await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/submissions/da443246-384d-673b-32db-bdba9d7f2b51/resources')
    .version('beta')
    .post(educationSubmissionResource);

```