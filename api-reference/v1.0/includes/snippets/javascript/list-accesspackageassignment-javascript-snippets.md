---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40ce2fdc2e4706bd91187d2619500a7ee56cf718
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346610"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignments = await client.api('/identityGovernance/entitlementManagement/assignments')
    .get();

```