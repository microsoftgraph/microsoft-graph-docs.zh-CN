---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3812e0cacd1503021d8d0e361b718604d6abc2104466fa1fabce55f161b1dc06
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/education/schools/delta')
    .get();

```