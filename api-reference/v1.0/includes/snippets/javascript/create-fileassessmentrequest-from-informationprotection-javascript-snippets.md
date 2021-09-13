---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97cd912cb9f7a6cd4b6110d5f602c409a020ed2693bed20a78a87cb77702175b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409741"
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
    .post(threatAssessmentRequest);

```