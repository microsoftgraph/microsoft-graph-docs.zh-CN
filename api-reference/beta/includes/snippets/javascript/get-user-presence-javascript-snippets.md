---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 598e96fb15c70d7aeeda0c7674582bff54224bbf050c077645335c61aff6ede1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101376"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let presence = await client.api('/users/66825e03-7ef5-42da-9069-724602c31f6b/presence')
    .version('beta')
    .get();

```