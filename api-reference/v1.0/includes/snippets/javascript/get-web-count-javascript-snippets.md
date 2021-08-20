---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2e320245658ea4fece2658d72094d3a08c672099a6444fe0e8eaf667ddafb94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378882"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applications = await client.api('/applications')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Web')
    .get();

```