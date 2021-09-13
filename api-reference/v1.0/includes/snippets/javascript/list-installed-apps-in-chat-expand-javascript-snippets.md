---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51af5c82015005b777b0299fcc86437c6d362da6d72c1797c5386908c9bb3b46
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904167"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/installedApps')
    .expand('teamsAppDefinition($expand=bot)')
    .get();

```