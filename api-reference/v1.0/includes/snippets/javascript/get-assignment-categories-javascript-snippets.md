---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e067f0f618703f81576d44e83549f2db9bd88f96
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507776"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let categories = await client.api('/education/classes/f4a941ff-9da6-4707-ba5b-0eae93cad0b4/assignments/9018ae7a-9953-4796-a152-4c54e0910922/categories')
    .get();

```