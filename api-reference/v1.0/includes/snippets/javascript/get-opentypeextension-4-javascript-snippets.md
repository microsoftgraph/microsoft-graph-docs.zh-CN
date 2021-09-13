---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a76e442669c5fa1bd93591f2af244d0562e803e4dd0d66e0383f30d6d72e5ec4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106788"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let extension = await client.api('/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate')
    .get();

```