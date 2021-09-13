---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a4e63cd63f27e449a9778f68cf95907b925c9cf3e75161eada4904b4ab81a0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162025"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo')
    .header('Accept-Language','fr')
    .get();

```