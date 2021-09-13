---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e608a377cdf814ac4d5bacf580beda8e9e975e600d24f8f7825d001dd6dc8e73
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let masterCategories = await client.api('/me/outlook/masterCategories')
    .get();

```