---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 099e2b89e5c60e79b9898ef011a062c98af15663ec85640fa1e889bcff81e254
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162447"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getApplicableContentTypesForList = await client.api('/sites/{siteId}/getApplicableContentTypesForList(listId='listId')')
    .version('beta')
    .get();

```