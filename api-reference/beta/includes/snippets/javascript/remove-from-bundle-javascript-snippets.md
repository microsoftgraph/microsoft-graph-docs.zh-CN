---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 929a37fc7674790c1a4f3f2d599b9338f6b1778c18edf8a7f7bbe92307071844
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106190"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drive/bundles/{bundle-id}/children/{item-id}')
    .version('beta')
    .delete();

```