---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9589635e712b8ca58ee33d88c80786dd729310d5
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46512349"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/items/{id}/workbook/comments')
    .version('beta')
    .get();

```