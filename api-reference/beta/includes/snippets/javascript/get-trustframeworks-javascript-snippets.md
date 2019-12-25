---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a567dbf7555c96115fa4aa5b2f5f61bfac47ccff
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "35716747"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/trustFramework/policies')
    .version('beta')
    .get();

```