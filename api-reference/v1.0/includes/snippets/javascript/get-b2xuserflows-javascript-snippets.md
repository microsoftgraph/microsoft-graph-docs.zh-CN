---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cee68a6c67af3de309b875bb85c077644dc6d1156ae592540c61f16bcc9cd6e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164132"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2xIdentityUserFlow = await client.api('/identity/b2xUserFlows/B2X_1_PartnerSignUp')
    .get();

```