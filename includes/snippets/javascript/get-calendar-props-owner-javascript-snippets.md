---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68d43de6ef37b91b7b427d6cd6217525d752a1124754d0c9e850b2905366cf4a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237057"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/AlexW@contoso.OnMicrosoft.com/calendar')
    .version('beta')
    .get();

```