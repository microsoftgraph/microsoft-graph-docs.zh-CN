---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 413ba95ef30358a7c9bff47fdee8117aecddaf46dcd6e416755021e73dd7ae26
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104797"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/synchronizationProfiles/{id}/reset')
    .version('beta')
    .post();

```