---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cd1da0f5ec05e7989ff03f8bcf05dfd3d47dd3b32103b957bff2982440a6f7c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277868"
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