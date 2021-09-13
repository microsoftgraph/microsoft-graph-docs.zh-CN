---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 821e9f11129bc4c9522688288622cf05c130facba16fae12ddecf0db719a7415
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279689"
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