---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 456a04e988af5fea194a014b54d1fee679c08f4e
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577950"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/reports/getM365AppUserCounts(period='D7')')
    .version('beta')
    .get();

```