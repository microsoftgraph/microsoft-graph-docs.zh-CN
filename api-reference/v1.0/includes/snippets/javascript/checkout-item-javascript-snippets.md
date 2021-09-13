---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d17c51a4195055aab83bdefad1b53a7ec55880e417890d0df40bbe966ab8c475
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106479"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drives/{drive-id}/items/{item-id}/checkout')
    .post();

```