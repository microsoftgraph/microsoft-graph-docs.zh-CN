---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f67a686ff4ac0f63cfbbdee45580066699b3d62
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395116"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contactMergeSuggestions = {
  isEnabled: false
};

await client.api('/me/settings/contactMergeSuggestions')
    .version('beta')
    .update(contactMergeSuggestions);

```