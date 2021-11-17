---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51506accafd5534824e9c4de42c4980882e38223
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "61021157"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let callRecord = await client.api('/communications/callRecords/getPstnCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)')
    .version('beta')
    .get();

```