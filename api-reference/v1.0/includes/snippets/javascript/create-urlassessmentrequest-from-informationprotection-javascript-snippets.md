---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1755b957f1e8135c9620b9dcf64f9192afb1787dd7a4960c9517c650d5623650
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409740"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const threatAssessmentRequest = {
  '@odata.type': '#microsoft.graph.urlAssessmentRequest',
  url: 'http://test.com',
  expectedAssessment: 'block',
  category: 'phishing'
};

await client.api('/informationProtection/threatAssessmentRequests')
    .post(threatAssessmentRequest);

```