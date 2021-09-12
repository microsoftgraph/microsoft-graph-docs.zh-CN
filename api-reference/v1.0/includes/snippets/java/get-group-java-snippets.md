---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d6c83a4ad9fe21b9bfd9c41752c504432a84bd7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59008310"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.sites("mycompany.sharepoint.com,8f03a01c-dcfa-4aaf-9be5-b3fb48e538c1,739084f3-c0fa-46ac-b7f8-13b344781ad0").termStore().groups("1FFD3F87-9464-488A-A0EC-8FB90911182C")
    .buildRequest()
    .get();

```