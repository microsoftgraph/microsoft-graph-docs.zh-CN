---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 583fb1ceba17b79de9aa73ec5e3eee16934f79f64dba32bf857a8185e50ccb90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161894"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const updateRecordingStatusOperation = {
  clientContext: 'clientContext-value',
  status: 'notRecording | recording | failed'
};

await client.api('/communications/calls/{id}/updateRecordingStatus')
    .version('beta')
    .post(updateRecordingStatusOperation);

```