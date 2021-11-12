---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e966b661aa1c7fa752670e0eb1df715a9273aae46a4e7255fbef97f29f8dd376
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/HeaderRowRange')
    .version('beta')
    .get();

```