---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5d405b3bcb05227181f1f53ca98292e77937748
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793752"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsTab = {
  displayName: 'My Contoso Tab',
  'teamsApp@odata.bind': 'https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8',
  configuration: {
    entityId: '2DCA2E6C7A10415CAF6B8AB6661B3154',
    contentUrl: 'https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView',
    websiteUrl: 'https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154',
    removeUrl: 'https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab'
  }
};

await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs')
    .version('beta')
    .post(teamsTab);

```