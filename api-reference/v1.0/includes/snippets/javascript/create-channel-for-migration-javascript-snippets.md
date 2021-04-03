---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 244a626b18b25929db6b1afcac24afd00e843b87
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508449"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
  '@microsoft.graph.channelCreationMode': 'migration',
  displayName: 'Import_150958_99z',
  description: 'Import_150958_99z',
  createdDateTime: '2020-03-14T11:22:17.067Z'
};

await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels')
    .post(channel);

```