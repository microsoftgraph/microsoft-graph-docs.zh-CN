---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc58e51d9cd3eeb320b14ad421fd381d575b8fa9b2a3100689e43a8d988906bc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106221"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscription = {
   expirationDateTime: '2016-11-22T18:23:45.9356913Z'
};

await client.api('/subscriptions/{id}')
    .update(subscription);

```