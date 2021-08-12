---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e702413fc2b9e7de9c38910f1d2e934f61a4487ac5c95c36133527b0492975b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54274541"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let monthlyPrintUsageByPrinter = await client.api('/print/reports/monthlyPrintUsageByPrinter')
    .version('beta')
    .get();

```