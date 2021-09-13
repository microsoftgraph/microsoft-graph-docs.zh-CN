---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f831a95910c7225dc811b4cd370b063b3e44ccce317f6c1133ba21c611327fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378465"
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
    .post(updateRecordingStatusOperation);

```