---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9041e3a520485c77f90b596d639dd426929b738bf45d82c041738f465450ba4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378703"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/dataBodyRange')
    .get();

```