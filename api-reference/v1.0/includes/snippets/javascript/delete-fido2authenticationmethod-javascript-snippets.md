---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adabbd1331d75d1b3139f9ff67ba665a260141880c42f2ff1d3c440991125fc4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2')
    .delete();

```