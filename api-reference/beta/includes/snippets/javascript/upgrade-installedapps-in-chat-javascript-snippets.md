---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb6b3ef8fa006365199faff5e8240ca0abe435eb09a4a547a8427b715973326e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278998"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=/upgrade')
    .version('beta')
    .post();

```