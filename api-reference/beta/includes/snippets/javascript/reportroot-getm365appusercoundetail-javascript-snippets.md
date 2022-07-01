---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b29fc80df530aa8eec994c685a2c26e621a907a
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66578001"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/reports/getM365AppUserDetail(period='D7')')
    .version('beta')
    .get();

```