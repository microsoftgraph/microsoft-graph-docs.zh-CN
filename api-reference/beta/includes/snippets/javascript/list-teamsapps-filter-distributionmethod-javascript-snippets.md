---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f27ae4bddb65bc373cb1c79245f09ae047f090fe87b0df64e42bba9e54bbb36
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215721"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsApps = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('distributionMethod eq \'organization\'')
    .get();

```