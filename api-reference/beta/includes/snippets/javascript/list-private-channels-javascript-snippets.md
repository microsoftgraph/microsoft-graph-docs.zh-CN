---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ceda2d436348d3905fd895274c4a621c8aa7e91d
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507294"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channels = await client.api('/teams/64c323f2-226a-4e64-8ba4-3e6e3f7b9330/channels')
    .version('beta')
    .filter('membershipType eq \'private\'')
    .get();

```