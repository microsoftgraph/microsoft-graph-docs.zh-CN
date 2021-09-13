---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bfd9b9972fab242eb7af83feb975fa0b30bd73f94ca5988db648ee4ec708da4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218407"
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
    .post(forward);

```