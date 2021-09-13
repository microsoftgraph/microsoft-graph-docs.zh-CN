---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3067bc9674508d6e3f7d32325813d7a231c404d03186e254e3b069c3d7944154
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104578"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let photos = await client.api('/groups/{id}/photos')
    .get();

```