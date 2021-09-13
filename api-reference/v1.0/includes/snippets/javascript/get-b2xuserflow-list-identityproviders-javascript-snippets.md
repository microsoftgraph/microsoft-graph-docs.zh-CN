---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 300e208021ab82d2a4103c16d7ca055c75e842d3acd45894c4ab8547ab82c870
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332140"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviders = await client.api('/identity/b2xUserFlows/B2X_1_Partner/identityProviders')
    .get();

```