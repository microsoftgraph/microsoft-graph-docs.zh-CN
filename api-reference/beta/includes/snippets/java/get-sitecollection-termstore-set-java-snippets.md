---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ec77bc0edbd46b768d36d21f290ce8aaca3abe3
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580475"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Set set = graphClient.sites("microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f").termStore().sets("8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f")
    .buildRequest()
    .get();

```