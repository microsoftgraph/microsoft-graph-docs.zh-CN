---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6dd11b38654645447a48940cdc167c36856121f274a2144f93ada5311407fdc8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158563"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applications = await client.api('/applications')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Web')
    .get();

```