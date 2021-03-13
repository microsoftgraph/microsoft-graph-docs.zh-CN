---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df2758ba026a89de176db9f404ae21dc46626e52
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774790"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsAppDefinition = [Zip file containing a Teams app package];

await client.api('/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions?requiresReview=true')
    .post(teamsAppDefinition);

```