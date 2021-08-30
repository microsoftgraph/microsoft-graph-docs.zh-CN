---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33e6faba06f494b86dfa4e50d49a5bfb0be4797a771ee3326672748ebc1c305a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902848"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsAppInstallation = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/installedApps/MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=')
    .version('beta')
    .get();

```