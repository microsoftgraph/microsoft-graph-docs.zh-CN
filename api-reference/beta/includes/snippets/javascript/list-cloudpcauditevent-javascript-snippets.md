---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a5f6711cf2d16113cf9eed6bec9773ece6418f68a0393f338f5b68b569875d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105947"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let auditEvents = await client.api('/deviceManagement/virtualEndpoint/auditEvents')
    .version('beta')
    .get();

```