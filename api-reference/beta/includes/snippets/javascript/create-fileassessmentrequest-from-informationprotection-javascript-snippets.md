---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acce92f3a6624fd0ace04870e9e10fb3879ae5c9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809240"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const threatAssessmentRequest = {
  '@odata.type': '#microsoft.graph.fileAssessmentRequest',
  expectedAssessment: 'block',
  category: 'malware',
  fileName: 'test.txt',
  contentData: 'VGhpcyBpcyBhIHRlc3QgZmlsZQ=='
};

await client.api('/informationProtection/threatAssessmentRequests')
    .version('beta')
    .post(threatAssessmentRequest);

```