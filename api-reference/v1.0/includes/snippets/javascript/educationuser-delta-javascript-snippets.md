---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 755d91e0cebe9d62604b10eb0cf8d0412c5881c95da3a9f8a544b046573f3204
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104979"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/education/users/delta')
    .get();

```