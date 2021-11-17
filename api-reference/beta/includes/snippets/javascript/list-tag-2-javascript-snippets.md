---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 789ff4b4d8b434a243842ba2f22fe4d19b234ab003c78033ff9902a9de0f31bc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220302"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let childTags = await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504/childTags')
    .version('beta')
    .get();

```