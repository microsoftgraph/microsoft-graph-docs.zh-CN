---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df3cca9243bba6959114eaa80449a65bac38224e209997f2c70c70c09cd17075
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219380"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/devices/{id}')
    .delete();

```