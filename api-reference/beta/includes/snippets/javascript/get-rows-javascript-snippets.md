---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ace08d8ea747eefc3499492de7f5b6d031b9398744f610d0dc98fb5498141f6b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164308"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rows = await client.api('/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/rows')
    .version('beta')
    .get();

```