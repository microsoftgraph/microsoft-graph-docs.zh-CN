---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 986f4236bc38cf185232bec6fa2be55117929dee
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580319"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.sites("microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f").termStore().groups("1FFD3F87-9464-488A-A0EC-8FB90911182C")
    .buildRequest()
    .get();

```