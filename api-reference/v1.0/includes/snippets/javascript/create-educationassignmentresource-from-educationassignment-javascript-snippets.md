---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3128fa02ad89d90d3c9f51c715ad05b3db087f54
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992792"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignmentResource = {
  distributeForStudentWork: 'false',
  resource: {
    displayName: 'Bing',
    link: 'https://www.bing.com',
    '@odata.type': 'educationLinkResource'
  }
};

await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/resources')
    .post(educationAssignmentResource);

```