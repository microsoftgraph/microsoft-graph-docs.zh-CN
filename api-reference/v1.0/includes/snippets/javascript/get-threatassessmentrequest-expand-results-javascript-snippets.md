---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c7b52111fdc54ace1635f9ca90ac39384447751
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42858856"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/informationProtection/threatAssessmentRequests/11922306-b25b-4605-ff0d-08d772fcf996')
    .expand('results')
    .get();

```