---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a73c612eaa1443cffcee10518008f062dd251cea00a7f72aa2e0c946c20577ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409668"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let licenseDetails = await client.api('/me/licenseDetails')
    .get();

```