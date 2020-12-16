---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03b663bbceca57557191a032d33a6e89a80657ce
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689643"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsTab = {
  displayName: "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  configuration: {
    entityId: "2DCA2E6C7A10415CAF6B8AB6661B3154",
    contentUrl: "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    websiteUrl: "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    removeUrl: "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
};

let res = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs')
    .version('beta')
    .post(teamsTab);

```