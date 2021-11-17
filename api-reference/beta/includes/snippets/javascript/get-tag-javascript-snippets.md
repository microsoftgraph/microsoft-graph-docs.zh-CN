---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a70fbecfca869d63c78b44dd376884c1a1ac1da2435d3eaf3ce2cebca4d1db5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161488"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tag = await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504')
    .version('beta')
    .get();

```