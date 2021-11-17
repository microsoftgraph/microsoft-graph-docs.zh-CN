---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b926545a07c8cd1c1328910fa6950ea8353e791751adb88d1ab4f1ba292afb96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277999"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.sites("microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f").termStore().groups("1FFD3F87-9464-488A-A0EC-8FB90911182C")
    .buildRequest()
    .get();

```