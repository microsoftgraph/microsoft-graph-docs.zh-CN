---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01148b9819d7ac6472db019bc77f101246a8437f52aec1cd2c98de1c4b0b0ad1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161461"
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
    .version('beta')
    .post(threatAssessmentRequest);

```