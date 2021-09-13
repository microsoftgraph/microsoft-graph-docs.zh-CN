---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69adc0fa5c7c58c3f2f91165a3cff2be0c509c5c469cfb7820ce888d567ac893
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332565"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  '@odata.type': 'microsoft.graph.mailSearchFolder',
  filterQuery: 'contains(subject, \'Analytics\')'
};

await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .update(mailFolder);

```