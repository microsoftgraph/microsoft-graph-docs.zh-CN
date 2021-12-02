---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11a4106c9928f8874ad40678d15398055b54516e01e04df846e4931f8e02cfd5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332711"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let int32 = await client.api('/contacts/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count')
    .version('beta')
    .get();

```