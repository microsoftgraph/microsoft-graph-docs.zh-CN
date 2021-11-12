---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ce26287f77093504288946c7be11a050ec6254cfadf67db10810d73a90de2dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163892"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let pivotTables = await client.api('/drive/root/workbook/worksheets/{id}/pivotTables')
    .version('beta')
    .get();

```