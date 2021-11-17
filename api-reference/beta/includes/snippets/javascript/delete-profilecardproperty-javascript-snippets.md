---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9433b8bf72c97c487263fe669abcb03b2010ae4e5e505b5372d233598e6ea057
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902489"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/organization/{organizationId}/settings/profileCardProperties/fax')
    .version('beta')
    .delete();

```