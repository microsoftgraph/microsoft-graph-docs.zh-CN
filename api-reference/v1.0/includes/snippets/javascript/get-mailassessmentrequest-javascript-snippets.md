---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fbe5d21d5fe928fa94bf22c81d595bfa4f3b6038d7a44e3f18ffce188364040
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221393"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threatAssessmentRequest = await client.api('/informationProtection/threatAssessmentRequests/49c5ef5b-1f65-444a-e6b9-08d772ea2059')
    .get();

```