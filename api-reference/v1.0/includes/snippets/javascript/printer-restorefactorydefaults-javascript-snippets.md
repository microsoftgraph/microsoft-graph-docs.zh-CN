---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c3d82eb8d682856572b43d4d7a9dab16ff9f90f00003ca9307ff7b3835e8ac1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218381"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{printerId}/restoreFactoryDefaults')
    .post();

```