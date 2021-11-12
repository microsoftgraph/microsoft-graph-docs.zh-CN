---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd6dc39ff2d39eb8105086357618b46b963111428cceac018c2ddd5373966780
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162088"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forward = {
  ToRecipients: [
      {
        emailAddress: {
          address: 'danas@contoso.onmicrosoft.com',
          name: 'Dana Swope'
        }
      }
     ],
  Comment: 'Dana, hope you can make this meeting.' 
};

await client.api('/me/events/{id}/forward')
    .version('beta')
    .post(forward);

```