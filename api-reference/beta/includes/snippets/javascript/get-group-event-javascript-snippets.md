---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 974e8e14dab93dcd3aded616b8b149c96b8853a406d478d6a62310782ae0ea69
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104787"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let event = await client.api('/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==')
    .version('beta')
    .get();

```