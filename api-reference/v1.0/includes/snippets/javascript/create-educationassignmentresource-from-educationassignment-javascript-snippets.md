---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b30e763acfb1e3926fb145646887b6656c3bc8b3e00400ecc31d2cce7e0c7811
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277233"
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