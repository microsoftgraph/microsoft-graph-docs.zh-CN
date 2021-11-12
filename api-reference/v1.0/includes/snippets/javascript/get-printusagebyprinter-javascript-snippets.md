---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32a7b439caefe3ac95cbb13219539c15f22188b9235b850a4708d53b32a91b8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163479"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printUsageByPrinter = await client.api('/reports/dailyPrintUsageByPrinter/{id}')
    .get();

```