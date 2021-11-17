---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9441541738e5778d6ac933ac3a2c72e7b80e9fc4db627cc61cef1f83feb0eda9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106377"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendar = await client.api('/me/calendar')
    .version('beta')
    .get();

```