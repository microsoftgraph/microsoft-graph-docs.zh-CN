---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ccf9f500b7662d7a3fe87dfc040eb695aa0760b4e51ec470c1f46e16e14fb29e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104973"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threatAssessmentRequests = await client.api('/informationProtection/threatAssessmentRequests')
    .get();

```