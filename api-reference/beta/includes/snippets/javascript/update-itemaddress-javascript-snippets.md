---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6a44387fb4f11c214571bb2ab6d34f4173ec8be2e7878dd21c5cab319d18472
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162797"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemAddress = {
  allowedAudiences: 'me',
  displayName: 'Secret Hideout',
};

await client.api('/users/{userId}/profile/addresses/{id}')
    .version('beta')
    .update(itemAddress);

```