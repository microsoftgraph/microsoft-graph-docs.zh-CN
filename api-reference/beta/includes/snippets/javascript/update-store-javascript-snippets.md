---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1fb8b554fe5db5a8023d0d6dafc497868a9fe6e4
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565788"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const store = {
  defaultLanguageTag: "en-US"
};

let res = await client.api('/termStore')
    .version('beta')
    .update(store);

```