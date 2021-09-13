---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5aa6b1978a8bae689690c70944bb8c4d7f4b3c3269e86b54d4bdbfa1f1a0a8cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218649"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscriptions = await client.api('/subscriptions')
    .get();

```