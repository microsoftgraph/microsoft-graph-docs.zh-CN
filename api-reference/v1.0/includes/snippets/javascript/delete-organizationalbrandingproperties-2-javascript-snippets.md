---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e786a339e99831704dfeef0942cb51d5a910218a3b36a9db8161b1727609ee8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215977"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr')
    .delete();

```