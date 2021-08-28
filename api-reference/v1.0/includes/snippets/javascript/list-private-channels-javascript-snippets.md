---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04f054994ee33ba57b9e0a345f05580110da92b0b5f12418c93f8087cad27cea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218416"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channels = await client.api('/teams/64c323f2-226a-4e64-8ba4-3e6e3f7b9330/channels')
    .filter('membershipType eq \'private\'')
    .get();

```