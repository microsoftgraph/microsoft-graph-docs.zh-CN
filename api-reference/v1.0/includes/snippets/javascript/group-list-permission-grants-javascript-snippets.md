---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fdca8d6281726d7bfd67675c9a62bfbfbb2f45edc10405b1021b6392e601d18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissionGrants = await client.api('/groups/14c981a4-dca9-4565-bae6-e13ada8861be/permissionGrants')
    .get();

```