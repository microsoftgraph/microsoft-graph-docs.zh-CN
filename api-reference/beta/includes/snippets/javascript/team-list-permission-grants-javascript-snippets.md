---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c53ef2b15b5ba16d18fa68e00c8b5cd38a0cd7091a389e3ab16310303e2f10b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903729"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissionGrants = await client.api('/teams/14c981a4-dca9-4565-bae6-e13ada8861be/permissionGrants')
    .version('beta')
    .get();

```