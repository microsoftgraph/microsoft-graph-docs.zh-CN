---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db6ab604fa4f0cbde8b6e223ae2d6dc7aafd5280e549eafee7a0a29236dae75e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215811"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let extension = await client.api('/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==='/extensions/Com.Contoso.Referral')
    .version('beta')
    .get();

```