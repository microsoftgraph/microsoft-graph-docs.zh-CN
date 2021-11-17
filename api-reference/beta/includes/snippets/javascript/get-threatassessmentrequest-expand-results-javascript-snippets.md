---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35067571dab91d7d343faca18e5e6d0280f800b3d449124e800d6ad3f54c0a41
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threatAssessmentRequest = await client.api('/informationProtection/threatAssessmentRequests/11922306-b25b-4605-ff0d-08d772fcf996')
    .version('beta')
    .expand('results')
    .get();

```