---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: faeda158f0f81ea1f85daf8b42cdd0de803baeffd370f4a73b7b252ab6cfe2da
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _boolean = {
  messageIds: ['MC172851', 'MC167983']
};

await client.api('/admin/serviceAnnouncement/messages/markRead')
    .version('beta')
    .post(_boolean);

```