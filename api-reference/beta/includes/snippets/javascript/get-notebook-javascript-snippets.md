---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b7f40a47ad6a88863cd26c76e8cb8a55750c9f6c5fed6318fa355a670dcb38b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332278"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let notebook = await client.api('/me/onenote/notebooks/{id}')
    .version('beta')
    .get();

```