---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 074ad7428ecda63f378291caaf197cc2fcc2fe9345cfc8ccb2456a0b77ff98da
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278681"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getActivitiesByInterval = await client.api('/drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')')
    .version('beta')
    .get();

```