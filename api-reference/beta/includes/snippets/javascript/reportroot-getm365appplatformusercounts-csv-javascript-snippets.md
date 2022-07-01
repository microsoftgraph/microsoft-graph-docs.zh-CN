---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 970a5d09088593801355c09a69855444671a864e
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577980"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/reports/getM365AppPlatformUserCounts(period='D7')')
    .version('beta')
    .get();

```