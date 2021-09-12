---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdd4722b758ac67a094b911df0722a6eb526eae294005f68faae6ce628b7cbbe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/usedRange')
    .get();

```