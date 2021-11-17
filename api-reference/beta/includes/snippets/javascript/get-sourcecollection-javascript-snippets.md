---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26620ebc067967bdda73f1339132232eb2d6d8c8ac48b9276c0d84bc654fb74f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sourceCollection = await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourcecollections/1a9b4145d8f84e39bc45a7f68c5c5119')
    .version('beta')
    .expand('lastEstimateStatisticsOperation')
    .get();

```