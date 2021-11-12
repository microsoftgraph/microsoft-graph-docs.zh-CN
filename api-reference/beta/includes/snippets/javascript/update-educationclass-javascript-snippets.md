---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 703f5803825ef945eafab15d6b6d90c0384747838efe21695f1584e9ab43abbd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333031"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
  description: 'History - World History 1',
  displayName: 'World History Level 1',
};

await client.api('/education/classes/11014')
    .version('beta')
    .update(educationClass);

```