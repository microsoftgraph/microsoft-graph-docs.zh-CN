---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f5d46da564e7fe7e6c662b450beeb523a98dadd26c2020a0b2775133faf4f8f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902351"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let alerts = await client.api('/security/alerts')
    .get();

```