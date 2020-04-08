---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f04bde6f73542c9920a6baa0a79a784a351c5660
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42815863"
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
    .post(threatAssessmentRequest);

```