---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ffed5bb13d9582cd2be31d9c20d46accaa83ca45b7df50a1a6fb9a26317b4bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378718"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/cell(row=5,column=6)')
    .get();

```