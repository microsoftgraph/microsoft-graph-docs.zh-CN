---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 684b29f2fa35adae6c654ed9d898fa9ecddad85a8a464bf4ae62bb459c704b8a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215828"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let extension = await client.api('/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate')
    .version('beta')
    .get();

```