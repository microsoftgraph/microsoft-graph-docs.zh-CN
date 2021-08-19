---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa4798f11b082042bcb5b57b5257c9f66de9fd76b171b133f0a3e95db3f4b926
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106710"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/contacts')
    .get();

```