---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48e3de64fe9ecf91f7f4c9a6d2503bf889b5884ba94c90a0bb4c4c030cff4ad2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903046"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threatAssessmentRequest = await client.api('/informationProtection/threatAssessmentRequests/723c35be-8b5a-47ae-29c0-08d76ddb7f5b')
    .version('beta')
    .get();

```