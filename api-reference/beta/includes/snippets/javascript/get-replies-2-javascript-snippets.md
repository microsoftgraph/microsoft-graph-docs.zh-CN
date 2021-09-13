---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac3e26e8f41ac0c850cc2e9ce8432587f6cf1184018c2d64e3793e8909a80f66
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221479"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let replies = await client.api('/drive/items/{id}/workbook/comments/{id}/replies')
    .version('beta')
    .get();

```