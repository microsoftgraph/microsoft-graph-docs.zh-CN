---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b632b466877d0c69be57d3a81dfd40562c2e0644405c77f68915daab0d329d77
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903536"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodConfiguration = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email')
    .get();

```