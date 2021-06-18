---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf6ff6bf7cc701da0fc9acf89a5325cf0506796e
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991418"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/c42f493f-42b4-4e7d-8148-af894cbc518b/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8')
    .delete();

```