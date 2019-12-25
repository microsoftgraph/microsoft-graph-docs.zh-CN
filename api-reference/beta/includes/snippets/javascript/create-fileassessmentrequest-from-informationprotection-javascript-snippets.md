---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 556ab7299743e5a2cac63d1472215ea7bcc68e0d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871766"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const threatAssessmentRequest = {
  @odata.type: "#microsoft.graph.fileAssessmentRequest",
  expectedAssessment: "block",
  category: "malware",
  fileName: "test.txt",
  contentData: "VGhpcyBpcyBhIHRlc3QgZmlsZQ=="
};

let res = await client.api('/informationProtection/threatAssessmentRequests')
    .version('beta')
    .post(threatAssessmentRequest);

```