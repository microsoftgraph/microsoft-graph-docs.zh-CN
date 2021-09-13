---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e4bd14919d5207c65cb1a27c5f43263670811cf7b7006dfde3c7a0f2a90e6cb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334121"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{item-id}/unfollow')
    .post();

```