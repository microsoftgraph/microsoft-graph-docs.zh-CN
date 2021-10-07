---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d4f5a1f32ff1bc8ea244ab228e566e09f07cf539ff87f7f96a1cda8acbf48d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsApps = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('appDefinitions/any(a:a/bot ne null)')
    .expand('appDefinitions($expand=bot)')
    .get();

```