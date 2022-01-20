---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1aced75dcce49435bc9d47c15142cb991eca7be0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106799"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customQuestions/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e')
    .version('beta')
    .delete();

```