---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e191215fad58d96a0fc27f946917c4a5168cd6ee9ac4202ac672fd2123baf934
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279155"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threatAssessmentRequest = await client.api('/informationProtection/threatAssessmentRequests/11922306-b25b-4605-ff0d-08d772fcf996')
    .expand('results')
    .get();

```