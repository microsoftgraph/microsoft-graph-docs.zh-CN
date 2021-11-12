---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe749b5e4c27a4b07d591bf0f0afd110c655492492ce8c619de38bb52ef60ee8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219846"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const store = {
  defaultLanguageTag: 'en-US'
};

await client.api('/termStore')
    .version('beta')
    .update(store);

```