---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51a6cc26ff6e8fcdc3ba5a4ffe20d52adc5d48ab
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871775"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const threatAssessmentRequest = {
  @odata.type: "#microsoft.graph.urlAssessmentRequest",
  url: "http://test.com",
  expectedAssessment: "block",
  category: "phishing"
};

let res = await client.api('/informationProtection/threatAssessmentRequests')
    .version('beta')
    .post(threatAssessmentRequest);

```