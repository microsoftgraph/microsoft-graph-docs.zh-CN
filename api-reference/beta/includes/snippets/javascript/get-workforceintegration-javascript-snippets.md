---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30ef5d52e84f0d71df52cbe80baa0c0498de1d69
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870535"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teamwork/workforceIntegrations/{workforceintegrationid}')
    .version('beta')
    .get();

```