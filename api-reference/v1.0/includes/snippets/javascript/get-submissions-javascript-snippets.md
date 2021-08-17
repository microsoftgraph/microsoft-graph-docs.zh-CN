---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92d00eeb7d0b15d921caa1d0c203ed62e7cb5d2099404212365fe57927ddbcc6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378443"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let submissions = await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions')
    .get();

```