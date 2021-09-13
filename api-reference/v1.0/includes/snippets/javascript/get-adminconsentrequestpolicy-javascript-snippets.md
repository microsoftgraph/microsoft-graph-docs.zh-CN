---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 242170fbf0be516677ddbeeb48b5090e58c27dd439753e441e7d84de61baf4c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378815"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let adminConsentRequestPolicy = await client.api('/policies/adminConsentRequestPolicy')
    .get();

```