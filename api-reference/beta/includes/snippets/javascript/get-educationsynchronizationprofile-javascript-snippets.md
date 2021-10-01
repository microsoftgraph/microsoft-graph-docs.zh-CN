---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfa2a3736462474dad96a5b9ec6b5e2033433ff0a2523df004fdbef20825bad3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332912"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationSynchronizationProfile = await client.api('/education/synchronizationProfiles/{id}')
    .version('beta')
    .get();

```