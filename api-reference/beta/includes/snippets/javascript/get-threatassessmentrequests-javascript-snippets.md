---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 952bba8ebc9263fb3835904067298e04aa8902094c8696ae17b8487a138f5275
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163407"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threatAssessmentRequests = await client.api('/informationProtection/threatAssessmentRequests')
    .version('beta')
    .get();

```