---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 920243bc9afa84279a7c0cdd85738d7b1caccbbfb42c3555f821c1df8818734b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163759"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/users/97a5a533-833d-494b-b543-c0afe026cb96/teamwork/installedApps')
    .version('beta')
    .filter('teamsApp/externalId eq \'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee\'')
    .expand('teamsAppDefinition')
    .get();

```