---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b31e055519568231b255c3fdca137cc60c4d8d75
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794079"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printOperation = await client.api('/print/operations/{id}')
    .version('beta')
    .get();

```