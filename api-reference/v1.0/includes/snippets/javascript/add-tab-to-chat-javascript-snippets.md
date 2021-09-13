---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65bf341a01baf61c485aeb8b9e3800c46ba2031109d6c523d53878b3dbfdc543
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274085"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsTab = {
  displayName: 'My Contoso Tab',
  'teamsApp@odata.bind': 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8',
  configuration: {
    entityId: '2DCA2E6C7A10415CAF6B8AB6661B3154',
    contentUrl: 'https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView',
    websiteUrl: 'https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154',
    removeUrl: 'https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab'
  }
};

await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs')
    .post(teamsTab);

```