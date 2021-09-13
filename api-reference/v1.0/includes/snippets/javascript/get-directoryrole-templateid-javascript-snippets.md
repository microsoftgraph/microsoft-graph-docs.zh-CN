---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24bf8e46fc431563c9f5ec7b08656b541e9f085f842081a5d72616a54626c589
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277677"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRole = await client.api('/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf')
    .get();

```