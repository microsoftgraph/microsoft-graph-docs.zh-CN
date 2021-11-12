---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2847fa42f9a49578748d7c17fb2a50c7bf0bffad2dfa7ad04017b61cd42ec1d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103867"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachments = await client.api('/me/messages/{id}/attachments')
    .version('beta')
    .get();

```