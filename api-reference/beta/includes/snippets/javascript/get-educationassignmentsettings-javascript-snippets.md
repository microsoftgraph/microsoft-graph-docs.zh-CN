---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e87c457c571acb5009268d1d1e4f17188ba7a0da
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763452"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignmentSettings = await client.api('/education/classes/f4a941ff-9da6-4707-ba5b-0eae93cad0b4/assignmentsettings')
    .version('beta')
    .get();

```