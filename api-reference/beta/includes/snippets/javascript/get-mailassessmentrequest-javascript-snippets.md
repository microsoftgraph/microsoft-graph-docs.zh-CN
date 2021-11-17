---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af05cb3eb10a1f481fbf3f66d27f549a0243212a4a8b551529a3015178c0c13d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903044"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threatAssessmentRequest = await client.api('/informationProtection/threatAssessmentRequests/49c5ef5b-1f65-444a-e6b9-08d772ea2059')
    .version('beta')
    .get();

```