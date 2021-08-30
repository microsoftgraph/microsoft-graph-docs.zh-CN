---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7c3b746fb552e883058ea3f6c649c1c40a3d149a91ec73416b3dab4655b66b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332411"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/teams/2ab9c796-2902-45f8-b712-7c5a63cf41c4/channels/19:20bc1df46b1148e9b22539b83bc66809@thread.skype/members')
    .version('beta')
    .get();

```