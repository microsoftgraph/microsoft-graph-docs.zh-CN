---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 639bcf3c13a373df09a2d195087bb13f7c75e084
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777143"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printSettings = {
  documentConversionEnabled: true
};

await client.api('/print/settings')
    .update(printSettings);

```