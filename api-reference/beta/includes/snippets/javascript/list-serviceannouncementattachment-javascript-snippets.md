---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c36b88cefa2cf8a03b0d32f573c7e5eb6b75e0c
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225973"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/admin/serviceAnnouncement/messages/MC54091/attachmentsArchive')
    .version('beta')
    .get();

```