---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1d4b37b02c801d889d1a1508a72a33416166da2a1b8684ca61a08fcd6e24c93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378845"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachments = await client.api('/me/events/{id}/attachments')
    .get();

```