---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c64e7903106f2ddc856a347bd0748b48735cc512c7f495990965735ac4e0d0d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273909"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members')
    .version('beta')
    .get();

```