---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 557dd44328cf162fd8c8b408e6f701d899fcf349037303637f8915f3e5a18cb2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277313"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskFolder = {
  name: 'Charity work'
};

await client.api('/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=')
    .version('beta')
    .update(outlookTaskFolder);

```