---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76e4616483e33b40cc78a040f303a9c233007fa1dc38a4f059cf240b8c199496
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378318"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printer = await client.api('/print/printers/{printerId}')
    .select('id,displayName,capabilities')
    .get();

```