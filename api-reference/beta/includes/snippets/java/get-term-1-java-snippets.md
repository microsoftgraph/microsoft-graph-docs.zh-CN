---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd4208c7ee6ed029b43287c29969aa4185ace7bf
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580429"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Term term = graphClient.sites("microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f").termStore().groups("1FFD3F87-9464-488A-A0EC-8FB90911182C").sets("8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f").terms("81be9856-9856-81be-5698-be815698be81")
    .buildRequest()
    .get();

```