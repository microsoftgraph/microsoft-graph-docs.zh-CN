---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70ff61389edd1d116bcd3a95c43cf29d3f6654fa9141fc84627e6936b250d8fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219984"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{id}/channels/{id}')
    .version('beta')
    .delete();

```