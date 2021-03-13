---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 932d3aadb46d436a917a20417c94b34f742ee2e9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782263"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schools = await client.api('/education/me/schools')
    .version('beta')
    .get();

```