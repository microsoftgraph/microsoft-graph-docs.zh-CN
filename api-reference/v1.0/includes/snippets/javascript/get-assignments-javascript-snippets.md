---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52387c21c55d97b58aaa89419f285ef68da4905478b9f2e606b640e241bda339
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104998"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignments = await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments')
    .get();

```