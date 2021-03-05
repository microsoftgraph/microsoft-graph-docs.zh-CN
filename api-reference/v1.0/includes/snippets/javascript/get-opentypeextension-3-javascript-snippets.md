---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d195d7864ce808dd04351be8cd69b5e9592d5cbe
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465340"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')
    .expand('extensions($filter=id%20eq%20\'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral\')')
    .get();

```