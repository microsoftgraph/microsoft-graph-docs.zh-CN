---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56e25f2fbca43c788422792f2707bd3e06a5d562369777a372997112e925db30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220011"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviders = await client.api('/identity/identityProviders')
    .get();

```