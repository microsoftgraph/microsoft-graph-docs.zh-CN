---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b91726ef9ea9e7bfdc3bf794dd40a58a2d3936be5c6e288047d3543ab8bc2990
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162224"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let fido2AuthenticationMethod = await client.api('/me/authentication/fido2Methods/-2_GRUg2-HYz6_1YG4YRAQ2')
    .version('beta')
    .get();

```