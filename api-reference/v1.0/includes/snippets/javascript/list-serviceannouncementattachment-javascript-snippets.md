---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc742c8095df82d3d8de4011c7d8851006580518
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225304"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/admin/serviceAnnouncement/messages/MC54091/attachmentsArchive')
    .get();

```