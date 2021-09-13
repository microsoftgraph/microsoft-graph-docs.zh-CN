---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bbe23e38b5839687c536344b7f38ce0f47df6957f6dfd20e21829d175911d31
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let site = await client.api('/sites/{site-id}')
    .get();

```