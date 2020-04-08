---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e92d26356fed2cd5e8a28634998dd4a315d69cc
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "40867151"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/informationProtection/threatAssessmentRequests/49c5ef5b-1f65-444a-e6b9-08d772ea2059')
    .version('beta')
    .get();

```