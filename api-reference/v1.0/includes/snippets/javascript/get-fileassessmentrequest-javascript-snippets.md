---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fca76fec10ce991dc6b2e1e0786b6848fa122a798148a05af130d404be58b7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221392"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threatAssessmentRequest = await client.api('/informationProtection/threatAssessmentRequests/18406a56-7209-4720-a250-08d772fccdaa')
    .get();

```