---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66f157dc8dbf5a9022a1b4847f4cb113207bb71ade9dc6fdd13c641f373e1f28
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273861"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let profileCardProperties = await client.api('/organization/{organizationId}/settings/profileCardProperties')
    .version('beta')
    .get();

```