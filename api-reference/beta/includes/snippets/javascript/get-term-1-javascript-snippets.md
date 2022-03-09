---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ebeb9c607e276be7ad8f08c30057ebbf23b670aeeda420a800a96a936a1aeca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333435"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let term = await client.api('/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f/terms/81be9856-9856-81be-5698-be815698be81')
    .version('beta')
    .get();

```