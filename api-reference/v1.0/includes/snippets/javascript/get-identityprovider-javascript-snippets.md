---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22365f68e2219a8a649fad98885db0fcbc8e623330df6c6cd7429b82bc8dfc14
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107023"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProvider = await client.api('/identityProviders/Amazon-OAuth')
    .get();

```