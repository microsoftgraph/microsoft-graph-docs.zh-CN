---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69933e71677cc71dcb598fa0a8687ea5198e0c8e9d56d270bacfcfaa36f376b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904285"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let windowsHelloForBusinessAuthenticationMethod = await client.api('/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2')
    .get();

```