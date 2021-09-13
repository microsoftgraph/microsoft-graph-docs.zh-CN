---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f651f37da5177eb557306cfc739763100b0907e392715ea8a98184c78b107e01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162578"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupSetting = await client.api('/groupSettings/{id}')
    .get();

```