---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a603052425e7768b47cf1a7bb099a0b897250dafb9d86943f94ca42e82c15f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277214"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{printerId}')
    .delete();

```