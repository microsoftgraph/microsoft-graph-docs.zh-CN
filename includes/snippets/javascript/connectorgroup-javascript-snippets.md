---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 255190ef59ae32da4bd842991e8780cc49ca466d
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142349"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectorGroup = {
@odata.id:"https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
};

let res = await client.api('/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83/connectorGroup/$ref')
    .version('beta')
    .put(connectorGroup);

```