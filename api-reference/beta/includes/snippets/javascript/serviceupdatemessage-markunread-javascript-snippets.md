---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2d4029f426e9282baf8edf76a6443a45d62525f386934e3feee1c7712573066
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220770"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _boolean = {
  messageIds: ['MC172851', 'MC167983']
};

await client.api('/admin/serviceAnnouncement/messages/markUnread')
    .version('beta')
    .post(_boolean);

```